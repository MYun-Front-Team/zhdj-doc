# 获取日账单列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取日账单列表

_**【应用场景】**_

获取日账单列表

_**【接口地址】**_

[http://ip:port/WalletQuery/DailyBill/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DailyBillList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BillDate | string | 否 | 账单日（如交易日+7天） |
| BillDealStatusList | array int | 否 | 账单处理状态：0待处理，10已处理，11已作废 |
| BillSettlementStatusList | array int | 否 | 账单结算状态：0未结算，1部分结算，10已结算 |
| BillStartDate | string | 否 | 账单开始日期 |
| BillEndDate | string | 否 | 账单结束日期 |
| ProductGroupCodeList | array string | 否 | 款号列表 |

> #### DailyBill_应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DailyBillSysNo | int | 是 | 系统编码 |
| BillDate | string | 是 | 账单日 |
| BillAmount | decimal\(18,2\) | 是 | 账单金额 |
| BillDealStatus | int | 是 | 账单处理状态：0待处理，10已处理，11已作废 |
| BillSettlementStatus | int | 是 | 账单结算状态：0未结算，1部分结算，10已结算 |
| TradeDate | string | 是 | 交易日 |
| AuditPerson | object | 否 | 核对人（简） |
| AuditTime | string | 否 | 审核时间 |
| DealPerson | object | 否 | 打款人员（简） |
| DealTime | string | 否 | 打款时间 |



