# 获取订单详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取订单详情

_**【应用场景】**_

获取订单详情

_**【接口地址】**_

[http://ip:port/OrderQuery/Order/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)OrderBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderBase | object | 是 | 基础字段 |
| OrderStatistic | object | 否 | 统计字段 |



