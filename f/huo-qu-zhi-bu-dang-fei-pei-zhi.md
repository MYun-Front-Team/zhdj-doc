# 获取支部党费配置 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取支部党费配置

_**【应用场景】**_

获取支部党费配置

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)GetPartyFeeConfig

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 支部系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RemindDay | int | 是 | 提醒天数 |
| FileUrl | string | 否 | 文件图片Path路径 |
| PaymentMethodList | string | 是 | 支付方式：0二维码，1在线；存储格式用“,"隔开。 |



