# 获取我的权限列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取我的权限列表

_**【应用场景】**_

获取我的权限列表

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)MyRightList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（同AdminSysNo） |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| ~~DataRangeSysNo~~ | ~~int~~ | ~~是~~ | ~~数据范围树编码~~ |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoleList | array list | 是 | 角色列表 |
| RightList | array list | 是 | 权限列表 |

#### RightList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RightSysNo | int | 是 | 权限系统编码 |
| RightName | string | 是 | 权限名称 |
| RightCode | string | 是 | 权限代码 |
| RightType | int | 是 | 权限类型：1模块，2子模块，3页面，4按钮 |

#### RoleList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoleSysNo | int | 是 | 角色系统编码 |
| RoleName | string | 是 | 角色名称 |
| RoleDesc | string | 是 | 角色描述 |



