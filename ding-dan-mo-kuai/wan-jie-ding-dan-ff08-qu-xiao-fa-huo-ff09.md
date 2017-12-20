# 完结订单（不发货） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

完结订单

_**【应用场景】**_

完结订单

注：1、删除剩余的订单锁；

2、标记订单为已发货状态和已完结状态；

3、购买数量修改为已发的数量，并修改订单金额和商品总金额等；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/F](http://ip:port/HMAction/River/AddRiver)inishOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| Remark | string | 否 | 完结理由 |

> #### 应答_数据_ {#请求数据}



