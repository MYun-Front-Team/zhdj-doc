# 获取订单支付方式统计 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取订单支付方式统计

_**【应用场景】**_

获取订单支付方式统计

_**【接口地址】**_

[http://ip:port/OrderQuery/Order/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)OrderPaymentStatistics

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 见搜索条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AmountSum | decimal\(18,2\) | 是 | 总金额 |
| PaymentStatisticsList | array object | 是 | 支付方式总金额列表 |

#### PaymentStatistics说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentType | int | 是 | 支付方式 |
| TotalAmount | decimal\(18,2\) | 是 | 支付总金额 |



