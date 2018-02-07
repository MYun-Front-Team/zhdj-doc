# 获取代理商详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取代理商详情

_**【应用场景】**_

获取代理商详情

_**【接口地址】**_

[http://ip:port/OrganizationQuery/Agent/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AgentBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否（二选一必须） | 组织系统编码 |
| AgentSysNo | int | 否（二选一必须） | 代理商系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AgentBase | object | 是 | 基础字段 |
| AgentStatistic | object | 否 | 统计字段 |



