# 获取待/已采购单详情（采购员）

##### _【功能说明】_ {#【功能说明】}

获取待/已采购单详情（采购员）

_**【应用场景】**_

获取待/已采购单详情（采购员）

_**【接口地址】**_  
[http://ip:port/OrderQuery/Order/GetBaidPurchaseOrderBySysNo](http://ip:port/OrderQuery/Order/GetBaidPurchaseOrderBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PurchaseOrderSysNo | int | 否 | 采购单流水编码（待采购详情不传，已采购详情只需要传这个） |
| SkuSysNo | int | 是 | SKU系统编码 |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| OrganizationFromSysNo | int | 是 | 采购员组织系统编码 |
| DataRangeSysNo | int | 是 | 采购员范围树编码（店铺树） |
| OrganizationToSysNo | int | 否 | 买家（商家）组织系统编码 |
| PersonSysNo | int | 否 | 买家（商家）人员系统编码 |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PurchaseOrderSysNo | int | 是 | 采购单流水编码 |
| SkuSysNo | int | 是 | SKU系统编码 |
| SkuName | string | 是 | SKU名称 |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| ProductGroupName | int | 是 | 款名称 |
| OrganizationFromSysNo | int | 是 | 采购员组织 |
| DataRangeSysNo | int | 是 | 采购员范围树编码（店铺树） |
| TotalAmount | decimal | 是 | 总金额 |
| UnitPrice | decimal | 是 | 单价 |
| SkuFileThumbnailUrlList | array\[string\] | 是 | SKU缩略图 |
| ProductFileThumbnailUrlList | array\[string\] | 是 | 款缩略图 |
| Items | array\[PurchaseOrderItem\] | 是 | 采购单明细 |

#### PurchaseOrderItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo | int | 是 | 采购单流水编码 |
| OrderSysNo | int | 是 | 订单明细编码 |
| Quantity | int | 是 | 订单明细数量 |
| TotalAmount | int | 是 | 总金额 |
| UnitPrice | decimal | 是 | 单价 |
| OrderCreateTime | string | 是 | 订单下单时间 |
| ReceiverName | string | 是 | 收货人 |
| ReceiverPhone | string | 是 | 收货电话 |



