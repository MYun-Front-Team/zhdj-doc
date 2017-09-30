# 获取角色列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取角色列表

_**【应用场景】**_

获取角色列表

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RoleList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| DataRangeSysNo | int | 是 | 数据范围树编码 |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoleSysNo | int | 是 | 角色系统编码 |
| RoleName | string | 是 | 角色名称 |
| RoleDesc | string | 否 | 角色描述 |
| SortNo | int | 是 | 排序 |



