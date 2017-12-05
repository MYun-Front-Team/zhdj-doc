# 创建在线支付 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

创建在线支付

_**【应用场景】**_

创建在线支付

注：1、在线支付支持的有：0余额，1支付宝，2微信，3银联

2、当IsNeedBalance=1时，先扣出全部可用余额后，在把剩余不足的钱用第三方付款；

_**【接口地址】**_

[http://ip:port/DealQuery/](http://ip:port/HMAction/River/AddRiver)Payment[/G](http://ip:port/HMAction/River/AddRiver)etPaymentUrl

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 订单系统编码 |
| PaymentType | int | 否 | 支付方式：0余额，1支付宝，2微信，3银联 |
| IsNeedBalance | int | 否 | 是否需要先扣余额：0否，1是 |
| OpenID | string | 否 | 微信OPENID |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentUrl | string | 是 | 支付方式系统编码 |



