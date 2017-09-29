# 根据模块，获取积分配置列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据模块，获取积分配置列表

_**【应用场景】**_

根据模块或模块类型等，在配置中心配置的积分赠送规则的列表。获取后，有业务操作人员在对应的模块中填写对应的积分数值。

_**【接口地址】**_

[http://ip:port/PointsQuery/Points/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PointsConfigsByModule

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块类型分类（类别树） |
| PointsType | int | 是 | 积分类型（枚举） |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsConfigSysNo | int | 是 | 积分配置系统编码 |
| OperateType | int | 是 | 动作类型（枚举） |
| OperateName | string | 是 | 动作名称 |
| PointsCycle | int | 是 | 赠送周期天数（用来判断一个周期内最多赠送次数，0无限） |
| MaxNum | int | 是 | 一个周期内最多赠送次数，0无限 |
| PointsValue | int | 否 | 默认值 |



