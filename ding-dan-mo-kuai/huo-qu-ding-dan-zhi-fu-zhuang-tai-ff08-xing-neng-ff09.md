# 获取订单支付状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取订单支付状态

_**【应用场景】**_

获取订单支付状态

_**【接口地址】**_

[http://ip:port/OrderQuery/Order/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PaymentStatusBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentStatus | int | 是 | 支付状态：0未支付，1部分支付，10已支付 |



