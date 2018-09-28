# 新增提现 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增提现

_**【应用场景】**_

新增提现

注：通过UserSysNo找到BizCompanyCode;

1、需判断可用余额和【可提现金额】是否充足；

_**【接口地址】**_

[http://ip:port/WalletAction/ReceiveCash/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddReceiveCash

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| WalletSysNo | int | 是 | 钱包系统编码 |
| ReceiveAmount | decimal（18，10） | 是 | 提现金额 |
| CardSysNo | int | 是 | 提现银行卡系统编码 |
| ReceiveTime | string | 否 | 提现时间 |
| ReceiveRemark | string | 否 | 提现申请说明 |
| IsOnline | int | 是 | 是否线上提现（0线下（走审核流程），1线上（无需审核，直接到银行卡、微信等））|
| ReceiveCashType| int | 否 | 线上提现方式 0银行卡，1微信,2支付宝 |
| WxOpenID| string | 否 | 微信OpenID |
| AliAccount| string | 否 | 支付宝账号 |






> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReceiveCashSysNo | int | 是 | 提现系统编码 |



