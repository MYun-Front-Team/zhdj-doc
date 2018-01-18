# 获取商家租用摊位列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取商家租用摊位列表

_**【应用场景】**_

获取商家租用摊位列表

_**【接口地址】**_

[http://ip:port/ShopQuery/Booth/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RentBoothList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家系统编码 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BoothBase | object | 是 | 基础字段 |
| BoothStatistic | object | 否 | 统计字段 |

#### SellerRent说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Seller | object | 是 | 商家实体 |
| ShopRentFee | decimal（18，2） | 是 | 店铺实际租金（元/月） |
| ShopDepositFee | decimal（18，2） | 是 | 店铺实际押金 |
| RentStartDate | string | 是 | 租用开始日期 |
| RentEndDate | string | 是 | 租用结束日期 |
| RentStatus | int | 是 | 租用状态：10租用，11解除 |
| Remark | string | 否 | 备注 |



