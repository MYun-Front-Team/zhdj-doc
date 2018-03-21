# 订单关联推送的优惠券

##### _【功能说明】_ {#【功能说明】}

订单关联推送的优惠券

_**【应用场景】**_

订单关联推送的优惠券

_**【接口地址】**_

http://ip:port/ShopQuery/Coupon/GetOrderPushCouponList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponCode| string| 是 | 优惠代码|
| CouponType | int | 是 | 优惠券类型：0自定义，1免邮，2邮费减免，3满减 |
| CouponSysNo | int | 是 | 优惠券编码 |
| Remark | string | 否 | 备注 |
| StartDate| datetime| 否 | 有效期开始时间 |
| EndDate| datetime| 否 | 有效期结束时间 |
| Coupon| object| 否 |优惠券|


















