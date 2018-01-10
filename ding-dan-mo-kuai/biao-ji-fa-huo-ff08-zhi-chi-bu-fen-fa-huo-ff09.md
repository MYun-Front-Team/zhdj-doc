# 标记发货（支持部分发货） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

标记发货

_**【应用场景】**_

标记发货，整个订单发货，该接口支持部分发货；

注：1、减少相应的订单锁；

2、创建发货单，并标记已发货状态；

3、如果发货数量与订购数量一致（每一个OrderItem）,则标记订单已发货，否则为部分发货；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/D](http://ip:port/HMAction/River/AddRiver)eliveryOrderItem

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| TrackingCompanySysNo | int | 是 | 快递公司系统编码 |
| TrackingNo | string | 是 | 单号 |
| DeliveryOrderItemList | array item | 是 | 订单商品发货数量 |

> #### DeliveryOrderItem说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo | int | 是 | 订单商品系统编码 |
| Quantity | int | 是 | 本次发货数量 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeliveryVoucherSysNo | int | 是 | 发货单系统编码 |



