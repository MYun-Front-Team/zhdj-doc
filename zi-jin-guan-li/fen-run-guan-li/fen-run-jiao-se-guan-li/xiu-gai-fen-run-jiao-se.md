# 修改分润角色 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改分润角色

_**【应用场景】**_

修改分润角色

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitRole/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditProfitRole

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRoleSysNo | int | 是 | 分润角色系统编码 |
| ~~ProfitRoleClassSysNo~~ | ~~int~~ | ~~否~~ | ~~分润角色分类（通用）~~ |
| ProfitRoleName | string | 否 | 分润角色名称 |
| IsEnable | int | 否 | 是否有效：0无，1有 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



