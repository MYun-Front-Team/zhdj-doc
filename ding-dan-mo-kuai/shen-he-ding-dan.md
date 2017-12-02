# 审核订单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

审核订单

_**【应用场景】**_

审核订单

注：1、只能审核自己组织的订单；

2、审核记录保存到”通用-审核“；

3、限制库存的SKU且订单锁数量不足的商品，可再次进行订单锁；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/A](http://ip:port/HMAction/River/AddRiver)uditOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| AuditStatus | int | 是 | 审核状态：0待审核，10已审核 |

> #### 应答_数据_ {#请求数据}



