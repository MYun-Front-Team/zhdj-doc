# 修改订单商品 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改订单商品

_**【应用场景】**_

修改订单商品

注：修改价格或数量会影响订单总金额，修改数量会影响订单锁库；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/E](http://ip:port/HMAction/River/AddRiver)ditOrderItem

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| EditStatus | int | 是 | 修改类型：0修改，1删除 |
| EditOrderItemList | array object | 是 | 修改订单商品列表 |

> #### EditOrderItem说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo | int | 是 | 订单商品系统编码 |
| RealPrice | decimal（18，2） | 否 | 实际价格 |
| Quantity | int | 否 | 实际购买数量 |

> #### 应答_数据_ {#请求数据}



