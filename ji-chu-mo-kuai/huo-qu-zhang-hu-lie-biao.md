# 获取账户列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取账户列表

_**【应用场景】**_

根据项目标识符和数据范围树系统编码，获取账户列表。

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AdminList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| DataRangeSysNo | int | 否 | 数据范围树编码（0则查询整个项目） |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AdminSysNo | int | 是 | 账户系统编码 |



