# 资金报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 26000100 | 资金报表 | 按支付方式维度 |
| 26000101 | 资金报表 | 按日期维度 |

> #### _请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |

> #### _应答数据 （PageResponseBase）【26000100】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentStatisticsList | array object | 是 | 支付统计 |
| OrderPaymentList | array object | 是 | 支付记录列表 |

#### PaymentStatistics说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentType | int | 是 | 支付方式 |
| TotalAmount | decimal\(18,2\) | 是 | 支付总金额 |

#### OrderPayment说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentType | int | 是 | 支付方式 |
| BuyerID | string | 否 | 买家支付ID |
| Amount | decimal\(18,2\) | 是 | 支付金额 |
| PayTime | string | 是 | 支付时间 |

#### _应答数据 （PageResponseBase）【26000101】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentStatisticsList | array object | 是 | 支付统计 |
| DailyPaymentList | array object | 是 | 日统计金额 |

#### DailyPayment说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderDate | string | 是 | 日期 |
| CashTotalAmount | decimal\(18,2\) | 是 | 现金总金额 |
| OnlineTotalAmount | decimal\(18,2\) | 是 | 线上总金额 |
| SettlementStatus | int | 是 | 结算状态（日期下的全部订单结算状态汇总） |



