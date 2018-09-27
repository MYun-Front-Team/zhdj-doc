#获取我的优惠券

##### _【功能说明】_ {#【功能说明】}

获取我的优惠券

_**【接口地址】**_
http://ip:port/ShopQuery/Coupon/GetMyCouponsList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 搜索条件 |
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
| Coupon | object | 否 | 优惠券 |



