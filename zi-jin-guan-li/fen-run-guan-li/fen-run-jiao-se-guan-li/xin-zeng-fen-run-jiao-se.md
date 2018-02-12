# 新增分润角色 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增分润角色

_**【应用场景】**_

新增分润角色

注：ModuleRelation与OrganizationSysNo/Register 二选一；

OrganizationSysNo与Register 二选一；

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitRole/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddProfitRole

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否（三选一） | 组织系统编码（与业务模块无关联时，由分润角色生成） |
| Register | object | 否（三选一） | 注册实体 |
| ModuleRelation | object | 否（三选一） | 模块关联 |
| ProfitRoleClassSysNo | int | 是 | 分润角色分类（通用） |
| ProfitRoleName | string | 是 | 分润角色名称 |
| IsEnable | int | 是 | 是否有效：0无，1有 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRoleSysNo | int | 是 | 系统编码 |



