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
| ~~DataRangeSysNo~~ | ~~int~~ | ~~是~~ | ~~数据范围树编码~~ |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| RoleLimit | object | 否 | 角色限制条件（见获取账户详情接口） |
| SourceType| int | 否 | 项目自定义来源（0所有，1销售，2交付，3运营等） |

> #### _Role应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoleSysNo | int | 是 | 角色系统编码 |
| RoleName | string | 是 | 角色名称 |
| RoleDesc | string | 否 | 角色描述 |
| RightList | array object | 否 | 权限列表（见获取账户详情接口） |
| SourceType| int | 否 | 项目自定义来源（0默认，1销售，2交付，3运营等） |
| IsSystem| int | 否 | 是否是系统角色 |


#### Right说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RightSysNo | int | 是 | 权限系统编码 |
| RightName | string | 是 | 权限名称 |
| RightCode | string | 是 | 权限代码 |
| RightType | int | 是 | 权限类型：1模块，2子模块，3页面，4按钮 |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleName | string | 否 | 模块名称 |



