#获取订单发货单详情

##### _【功能说明】_ {#【功能说明】}

获取订单发货单详情

_**【应用场景】**_

获取订单发货单详情

_**【接口地址】**_
http://ip:port/OrderQuery/Delivery/GetOrderDeliveryBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderDeliverySysNo| int | 否 |系统编码 |


> #### 应答_数据（数组）_ {#请求数据}


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderDeliverySysNo| int | 是 | 系统编码 |
| DeliveryStatus| int | 是 | 发货状态|
| DeliveryDate| string| 是 | 发货时间 |
| TrackingNo| string| 是 | 快递公司 |
| TrackingCompany | object | 否 | 快递公司实体（见通用） |
| DeliveryOrderItems| array DeliveryOrderItem| 否 | 发货单明细 |


 #### DeliveryOrderItem


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo| int | 是 | 明细系统编码 |
| Quantity| int | 是 | 数量|
| SkuSysNo| int | 是 | SKU系统编码|
| SkuName| string| 是 | SKU名称|
| ProductGroupCode| string| 是 |款号|
| Amount| decimal| 是 | 金额|








