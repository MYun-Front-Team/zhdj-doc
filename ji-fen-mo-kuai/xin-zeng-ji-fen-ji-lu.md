# 新增业务积分 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

新增业务积分

_**【应用场景】**_

新增业务积分，该接口由端调用，应用场景如下载、系统管理员调整积分等。

注意：当调整积分时，积分变化值和有效期才是必填项。

当下载动作时，积分值是通过业务积分值配置表中获取，所以接口参数中不提供积分值配置系统编码。

备注也为必填项，显示在积分日志列表的积分变化原因或说明中。

积分人员系统编码通过InUserSysNo获取。

_**【接口地址】**_

[http://ip:port/PointsAction/Points/AddP](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)oints

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OperateType | int | 是 | 积分新增类型：12调整积分，5下载 |
| OwnerSysNo | int | 是 | 积分所有者系统编码（获取支部积分时必填） |
| PointsType | int | 是 | 积分类型（枚举） |
| ChangePointsValue | int | 否（调整积分时必填） | 积分变化值（区分正负） |
| SourceTime | string | 否（调整积分时必填） | 有效期开始时间（小于当前时间即冻结） |
| ~~ConfigValueSysNo~~ | ~~int~~ | ~~是~~ | ~~积分值配置系统编码~~ |
| ModuleSourceSysNo | int | 否（调整积分时非必填） | 模块来源系统编码 |
| Remark | string | 是 | 备注 |

####  {#应答数据-}



