# CPS获取订单列表

##### _【功能说明】_ {#【功能说明】}

CPS获取订单列表

_**【应用场景】**_

CPS获取订单列表

_**【接口地址】**_

http://ip:port/OrderQuery/Order/GetCPSOrderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围编码列表（店铺树） |
| OrganizationToSysNo | int | 否 | 买家组织系统编码 |
| PersonSysNoList | array int | 否 | 买家人员系统编码 |
| KeyWord | string | 否 | 关键字搜索（订单号/收货人/收货手机） |
| PaymentStatusList | array int | 否 | 支付状态 |
| CancelStatusList | array int | 否 | 取消状态 |
| FinishStatusList | array int | 否 | 完结状态 |
| SettlementStatusList | array int | 否 | 结算状态 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| OrderCode | string | 是 | 订单号 |
| OrderItemList | array object | 否 | 订单商品列表 |
| OrderAmountList | array object | 否 | 订单金额列表 |
| CreateTime | datetime | 否 | 创建时间|
| CPSSysNo | int | 否 | CPS系统编码|
| CPSCode | int | 否 | CPS编码|
| CreateTime| datetime| 否 | 三方订单下单时间|








