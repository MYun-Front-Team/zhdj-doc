# 新增支付记录 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增支付记录

_**【应用场景】**_

新增支付记录

注：新增本次支付记录后，累计已支付的总金额，与订单总金额判断，订单的支付状态；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/A](http://ip:port/HMAction/River/AddRiver)ddOrderPayment

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| PaymentType | int | 是 | 支付方式：0余额，1支付宝，2微信支付，3银联，4线下 |
| TradeNo | string | 是 | 交易号 |
| TotalFee | decimal\(18,2\) | 是 | 交易金额 |
| PayTime | string | 否 | 支付时间 |
| BuyerID | string | 否 | 买家帐户 |
| SellerID | string | 否 | 卖家帐户 |
| Remark | string | 否 | 完结理由 |

> #### 应答_数据_ {#请求数据}



