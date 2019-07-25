# 设置订单支付状态 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置订单支付状态

_**【应用场景】**_

设置订单支付状态

注：记录log日志；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/S](http://ip:port/HMAction/River/AddRiver)etOrderPaymentStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| PaymentStatus | int | 是 | 支付状态：0未支付，1部分支付，2已汇款待确认10已支付 |
| Remark | string | 否 | 备注 |



> #### 应答_数据_ {#请求数据}



