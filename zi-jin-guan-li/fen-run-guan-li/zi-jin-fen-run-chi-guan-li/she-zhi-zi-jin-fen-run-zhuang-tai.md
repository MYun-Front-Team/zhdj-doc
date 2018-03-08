# 设置资金分润状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置资金分润状态

_**【应用场景】**_

设置资金分润状态

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitPool/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etProfitPoolStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolSysNo | int | 是 | 系统编码 |
| ProfitPoolStatus | int | 是 | 分润池状态：10已分润，11已作废 |
| ProfitRuleSysNo | int | 否 | 分润规则系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



