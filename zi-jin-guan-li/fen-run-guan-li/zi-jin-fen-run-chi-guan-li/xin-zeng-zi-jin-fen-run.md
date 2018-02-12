# 新增资金分润 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增资金分润

_**【应用场景】**_

新增资金分润

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitPool/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddProfitPool

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 付款方组织系统编码 |
| ModuleRelation | object | 否 | 模块关联 |
| AgentType | int | 否 | 冗余代理商类型 |
| AgentPCDCode | string | 否 | 冗余代理省市区Code |
| AgentPCDDescription | string | 否 | 冗余代理省市区描述 |
| ProfitPoolSourceType | int | 是 | 分润资金来源：0线上，1线下 |
| ProfitPoolType | int | 是 | 资金类型：0代理费，1广告费，2会员费，3交易佣金 |
| ProfitPoolAmount | decimal（18，2） | 是 | 分润资金 |
| ProfitRuleSysNo | int | 否 | 分润规则系统编码 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolSysNo | int | 是 | 系统编码 |



