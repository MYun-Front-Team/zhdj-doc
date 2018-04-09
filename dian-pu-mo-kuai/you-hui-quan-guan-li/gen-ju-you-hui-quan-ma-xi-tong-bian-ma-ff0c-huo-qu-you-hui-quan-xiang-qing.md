# 根据优惠券码系统编码，获取优惠券详情

##### _【功能说明】_ {#【功能说明】}

根据订单添加实体获取可用优惠券

_**【接口地址】**_

http://ip:port/ShopQuery/Coupon/GetCouponsByCouponCodeSysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponCodeSysNo | int | 是 | 优惠券码系统编码 |
| Limit | object | 否 | 限制条件 |


> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponCode | string | 是 | 优惠代码 |
| CouponType | int | 是 | 优惠券类型：0自定义，1免邮，2邮费减免，3满减 |
| CouponSysNo | int | 是 | 优惠券编码 |
| Remark | string | 否 | 备注 |
| StartDate | datetime | 否 | 有效期开始时间 |
| EndDate | datetime | 否 | 有效期结束时间 |
| IsOverDue | int | 是 | 是否过期：0否，1是 |
| ShareStatus | int | 否 | 分享状态0未分享，1已分享，10已领取|
| Coupon | object | 否 | 优惠券 |
| Person | object | 否 | 优惠券拥有者|






