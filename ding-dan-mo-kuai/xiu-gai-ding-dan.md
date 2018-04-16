# 修改订单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改订单

_**【应用场景】**_

修改订单

注：只能修改订单主体信息；

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/E](http://ip:port/HMAction/River/AddRiver)ditOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |
| PaymentType | int | 否 | 支付方式（枚举） |
| TrackingCompanySysNo | int | 否 | 期望快递公司系统编码 |
| ReceiverName | string | 否 | 收货人 |
| ReceiverPhone | string | 否 | 收货电话 |
| ReceiverAddress | string | 否 | 收货地址 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| IsNeedBill | int | 否 | 是否需要发票 |
| BillName | string | 否 | 发票抬头 |
| BillType | int | 否 | 发票类型：1企业，2机构，3个人 |
| OrderRemark | string | 否 | 订单买家备注 |
| DeliveryRemark | string | 否 | 订单卖家备注 |
|IsDoortodoor|int | 是 | 是否上门服务|



> #### 应答_数据_ {#请求数据}



