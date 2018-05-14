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
| CPSValidList| array int | 否 | CPS是否失效（0有效，1失效） |
| FinishStatusList | array int | 否 | 完结状态 |




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

> ###OrderItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 系统编码 |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| SkuSysNo| int | 是 | 款系统编码 |
| SourceSkuCode| string | 是 | 三方来源SKUID |
| SkuName| int | 是 | SKU名称|
| FileThumbnailUrlList| array[string]| 是 | SKU图片 |
| RealPrice| decimal| 是 | 价格|
| Quantity| int | 否 | 数量 |
| CPSCommission| decimal | 否 | 佣金 |
| CPSValid| int| 否 | CPS是否失效（0有效，1失效）|
| CPSValidRemark| string | 否 |失效备|
| CPSCode | int | 否 | CPS编码|
| CreateTime| datetime| 否 | 三方订单下单时间|

> ###OrderAmount

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 系统编码 |
| AmountType | int | 是 | 业务逻辑自定义金额类型 6实际支付总金额，9原始订单总金额，10当前商品总金额, 12CPS佣金 |
| Amount | decimal（18，2） | 是 | 金额 |
| Remark | string | 否 | 备注 |


