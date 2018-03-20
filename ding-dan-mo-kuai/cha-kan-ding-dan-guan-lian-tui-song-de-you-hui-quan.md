# 订单关联推送的优惠券

##### _【功能说明】_ {#【功能说明】}

订单关联推送的优惠券

_**【应用场景】**_

订单关联推送的优惠券

_**【接口地址】**_

http://ip:port/OrderQuery/Order/GetOrderPushCouponList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderCouponSysNo | int | 是 | 订单支付系统编码 |
| CouponType | int | 是 | 优惠券类型：0自定义，1免邮，2邮费减免，3满减 |
| CouponSysNo | int | 是 | 优惠券编码 |
| CouponCode | string | 否 | 优惠代码 |
| CouponAmount | decimal（18，2） | 是 | 优惠金额\(减免金额\) |
| Remark | string | 否 | 备注 |





