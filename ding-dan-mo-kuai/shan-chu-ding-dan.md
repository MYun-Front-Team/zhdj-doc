# 取消订单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

取消订单

_**【应用场景】**_

取消订单

注：已审核订单不允许取消，取消订单把CancelStatus=10，把备注写入到日志中；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/C](http://ip:port/HMAction/River/AddRiver)ancelOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| CancelRemark | string | 否 | 取消备注 |

> #### 应答_数据_ {#请求数据}



