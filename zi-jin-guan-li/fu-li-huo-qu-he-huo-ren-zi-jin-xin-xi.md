# 福狸获取合伙人资金信息

##### _【功能说明】_ {#【功能说明】}

福狸获取合伙人资金信息

_**【应用场景】**_

福狸获取合伙人资金信息

_**【接口地址】**_

http://ip:port/WalletQuery/Wallet/GetFLPartnerWallet

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| PersonSysNo| int | 是 | 人员系统编码 |



> #### _应答数据 _ {#应答数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 否 | 佣金信息 |


> #### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Commission| decimal | 否 | 效果预估佣金 |
| FinishCommission| decimal（18，10） | 是 | 结算效果预估 |
| AvailableReceiveCashAmount| decimal | 否 | 可提现金额 |


