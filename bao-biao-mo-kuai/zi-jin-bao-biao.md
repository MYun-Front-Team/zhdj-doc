# 资金报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 26000100 | 资金报表 | 按支付方式维度 |
| 26000101 | 资金报表 | 按日期维度 |
| ~~26000102~~ | ~~资金报表~~ | ~~按可提现维度（订单销售的金额）~~ |
| 26000103 | 分润报表 | 按分润来源 |
| 26000104 | 资金报表 | 工商行对账详情 |
| 26000105 | 资金报表 | 工商行对账汇总 |


> #### _请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |
| ProfitModuleSourceType | int | 是 | 分润来源 |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| PersonName| string | 否 |姓名 |
| ModuleSourceType| int | 否 | 费用类型：26001一卡通充值，39008缴费明细|
| PaidName| string | 否 |项目名称 |


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
| PointRealWorth| decimal\(18,2\) | 是 | 积分支付换算金钱总金额 |
| PayTime | string | 是 | 支付时间 |
| OrderSysNo | int | 是 | 订单系统编码 |

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
| PointRealWorth| decimal\(18,2\) | 是 | 积分支付换算金钱总金额 |
| SettlementStatus | int | 是 | 结算状态（日期下的全部订单结算状态汇总） |

#### _应答数据 （PageResponseBase）【26000103】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitStatisticsList | array object | 是 | 分润统计 |
| WalletLogList | array object | 是 | 分润明细 |

#### 应答数据 （ProfitStatistics）
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitModuleSourceType | int | 是 | 分润来源（26008会员费分润，23001订单分润，26010代理费分润，304充值积分） |
| TotalAmount| decimal | 是 | 统计金额 |

#### 应答数据 （WalletLog）
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitModuleSourceType | int | 是 | 分润来源（26008会员费分润，23001订单分润，26010代理费分润，304充值积分） |
| Amount | decimal | 是 | 金额 |
| TradeDescription| string| 是 | 描述 |


#### _应答数据 （PageResponseBase）【26000104】
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo| int | 是 | 订单编号 |
| PersonName| string | 否 |姓名 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| PaymentAmount| decimal| 否 |支付金额 |
| ModuleSourceType| int | 否 | 费用类型：26001一卡通充值，39008缴费明细|
| PaidName| string | 否 |项目名称 |
| PaymentAmount| decimal| 否 |支付金额 |
| PaidTime| datetime| 否 |支付时间 |

#### _应答数据 （PageResponseBase）【26000105】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaidTime| datetime| 否 |支付时间 |
| PaymentAmount| decimal| 否 |支付金额 |
| OrderCount| int| 否 |笔数 |

> #### 应答数据 PageResponseStatistic 【26000105】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentAmount| decimal| 否 |支付金额 |
| OrderCount| int| 否 |笔数 |


