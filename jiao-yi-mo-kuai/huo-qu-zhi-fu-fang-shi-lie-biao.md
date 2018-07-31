# 获取支付方式列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取支付方式列表

_**【应用场景】**_

获取支付方式列表

注：当根据OrganizationSysNo或DataRangeSysNo，获取结果为空时，返回系统默认的支付方式。

_**【接口地址】**_

[http://ip:port/DealQuery/](http://ip:port/HMAction/River/AddRiver)Payment[/G](http://ip:port/HMAction/River/AddRiver)etPaymentList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| PaySource | int | 是 | 支付来源：1PC，2APP，3H5，4微信 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentSysNo | int | 是 | 支付方式系统编码 |
| PaymentType | int | 是 | 支付方式：0余额，1支付宝，2微信，3银联，4线下，5刷卡,6积分,7联动支付，8工行E支付，9禾商行 |
| PaymentName | string | 是 | 支付方式名称 |
| PaymentDesc | string | 否 | 支付方式描述 |
| PaymentUrl | string | 否 | 支付方式Logo |
| PaymentList | array object | 否 | 子支付方式列表 |



