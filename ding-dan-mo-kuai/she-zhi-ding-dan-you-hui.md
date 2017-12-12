# 设置订单优惠 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置订单优惠

_**【应用场景】**_

设置订单优惠

注：目前仅支持优惠类型如下；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/S](http://ip:port/HMAction/River/AddRiver)etOrderAmount

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| AmountType | int | 是 | 类型：7客服优惠金额，8运费优惠金额 |
| Amount | decimal\(18,2\) | 是 | 优惠金额 |
| Remark | string | 否 | 备注 |

> #### 应答_数据_ {#请求数据}



