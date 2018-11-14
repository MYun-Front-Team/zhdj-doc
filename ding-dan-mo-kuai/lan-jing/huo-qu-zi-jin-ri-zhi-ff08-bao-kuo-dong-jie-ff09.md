# 获取钱包日志列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取钱包日志列表

_**【应用场景】**_

获取钱包日志列表

_**【接口地址】**_


http://ip:port/WalletQuery/Wallet/GetLJWalletLog

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WalletSysNo | int | 是 | 钱包系统编码 |
| ModuleSourceTypeList |array int | 否|23003采购单 26004提现 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WalletLogSysNo | int | 是 | 钱包日志系统编码 |
| TradeType | int | 是 | 交易类型：0支付，1充值，2提现，3转账，4退款,5冻结 |
| TradeDescription | string | 是 | 交易描述 |
| PaymentType | int | 是 | 交易工具：0线下 1-支付宝、2-微信，3-钱包余额支付，4-银行卡支付 |
| TradeNo | string | 否 | 交易流水号 |
| Amount | decimal（18，10） | 是 | 成交金额 |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |


