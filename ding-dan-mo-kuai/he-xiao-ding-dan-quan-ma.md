# 核销订单券码 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

核销订单券码

_**【应用场景】**_

核销订单券码

注：到店消费，核销订单券码逻辑；

1、根据券码判断是否具有有效性（订单有效，券码没有被使用过）；

2、核销之后，需记录订单日志（操作类型为消费）；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/W](http://ip:port/HMAction/River/AddRiver)riteOffOrderCouponCode

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| CouponCode | string | 是 | 券码 |

> #### 应答_数据_ {#请求数据}



