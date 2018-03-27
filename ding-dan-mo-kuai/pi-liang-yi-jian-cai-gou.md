# 批量一件采购（采购员）

##### _【功能说明】_ {#【功能说明】}

批量一件采购（采购员）

_**【应用场景】**_
批量一件采购（采购员）

_**【接口地址】**_

http://ip:port/OrderAction/Order/DeliveryPurchaseOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | SKU系统编码 |
| OrganizationFromSysNo | int | 是 | 采购员组织系统编码 |
| DataRangeSysNo | int | 是 | 采购员范围树编码（店铺树） |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |








