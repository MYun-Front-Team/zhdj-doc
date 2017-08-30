# 新增业务积分 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

新增业务积分

_**【应用场景】**_

新增业务积分

_**【接口地址】**_

[http://ip:port/UMAction/Point/AddP](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)oints

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType | int | 否（与积分所有者系统编码形成联合主键） | 积分类型 |
| CustomerSysNo | int | 否 | 积分所有者系统编码 |
| PointsSysNo | int | 否（与上述联合主键二选一必填） | 积分主键 |
| ChangePointsValue | int | 是 | 积分变化值（区分正负） |
| SourceTime | int | 是 | 有效期开始时间（小于当前时间即冻结） |
| SourceType | int | 是 | 来源类型 |
| SouceVoucherNo | string | 是 | 来源单据号 |
| Memo | string | 是 | 备注 |

####  {#应答数据-}



