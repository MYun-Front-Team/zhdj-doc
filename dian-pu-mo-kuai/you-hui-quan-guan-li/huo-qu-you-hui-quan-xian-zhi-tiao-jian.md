# 获取优惠券限制条件 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取优惠券限制条件

_**【应用场景】**_

获取优惠券限制条件

_**【接口地址】**_

[http://ip:port/ShopQuery/Coupon/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)CouponCoditionsBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponSysNo | int | 是 | 优惠券系统编码 |
| CoditionLimit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CategoryList | array object | 否 | 商品类别列表 |
| CustomerLevelList | array object | 否 | 客户等级列表 |

#### CoditionLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowCategoryList | int | 否 | 是否显示商品类别列表 |
| IsShowCustomerLevelList | int | 否 | 是否显示客户等级列表 |



