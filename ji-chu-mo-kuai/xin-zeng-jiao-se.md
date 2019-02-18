# 新增角色 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增角色

_**【应用场景】**_

新增角色

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddRole

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| ~~DataRangeSysNo~~ | ~~int~~ | ~~是~~ | ~~数据范围树编码~~ |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| RoleName | string | 是 | 角色名称 |
| RoleDesc | string | 否 | 角色描述 |
| SortNo | int | 否 | 排序 |
| SourceType| int | 否 | 项目自定义来源（0默认，1销售，2交付，3运营等） |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoleSysNo | int | 是 | 角色系统编码 |



