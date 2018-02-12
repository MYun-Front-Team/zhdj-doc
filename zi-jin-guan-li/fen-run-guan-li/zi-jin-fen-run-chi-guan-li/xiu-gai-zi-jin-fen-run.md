# 修改资金分润 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改资金分润

_**【应用场景】**_

修改资金分润

注：待分润状态时可修改；

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitPool/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditProfitPool

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolSysNo | int | 是 | 系统编码 |
| ProfitPoolSourceType | int | 是 | 分润资金来源：0线上，1线下 |
| ProfitPoolType | int | 是 | 资金类型：0代理费，1广告费，2会员费，3交易佣金 |
| ProfitPoolAmount | decimal（18，2） | 是 | 分润资金 |
| ProfitRuleSysNo | int | 否 | 分润规则系统编码 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



