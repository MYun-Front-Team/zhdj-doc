# 获取Saas项目号记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取Saas项目号记录

_**【应用场景】**_

获取Saas项目号记录

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BizCompanyCodeBySaasKey

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SaasKey | string | 是 | SaasKey值 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SaasSysNo | int | 是 | 系统编码 |
| SaasKey | string | 是 | SaasKey值 |
| BizCompanyCode | string | 是 | 项目标识符 |
| NewCompanyCode | string | 是 | 项目号 |



