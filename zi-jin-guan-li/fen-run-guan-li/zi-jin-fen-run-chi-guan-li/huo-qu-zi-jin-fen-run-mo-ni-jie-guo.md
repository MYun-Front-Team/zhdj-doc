# 获取资金分润模拟结果 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取资金分润模拟结果

_**【应用场景】**_

获取资金分润模拟结果

_**【接口地址】**_

[http://ip:port/WalletQuery/ProfitPool/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ProfitPoolResultBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolSysNo | int | 是 | 系统编码 |
| ProfitRuleSysNo | int | 是 | 分润规则系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitTotalAmount | decimal（18，2） | 是 | 可分润总金额 |
| ProfitPoolDetailList | array object | 否 | 资金分润明细列表 |



