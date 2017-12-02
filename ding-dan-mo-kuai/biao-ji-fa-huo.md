# 标记发货（简版） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

标记发货

_**【应用场景】**_

标记发货，整个订单发货，该接口不支持部分发货；

注：1、把全部订单锁数量减去物理库存后，清空订单锁，标记订单已发货；

2、创建发货单，并标记已发货状态；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/D](http://ip:port/HMAction/River/AddRiver)eliveryOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| TrackingCompanySysNo | int | 是 | 快递公司系统编码 |
| TrackingNo | string | 是 | 单号 |

> #### 应答_数据_ {#请求数据}



