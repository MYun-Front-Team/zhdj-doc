# 获取钱包提现明细
##### _【功能说明】_ {#【功能说明】}

获取钱包提现明细

_**【应用场景】**_
获取钱包提现明细

_**【接口地址】**_

http://ip:port/RecruitQuery/Wallet/GetNPLWalletCashList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserName | string | 是 |姓名|
| TransferTime | string | 是 |姓名|
| TransferOrdid | string | 是 |交易流水号|
| OrderAmt | string | 是 |订单金额|
| TransferAmt | string | 是 |交易金额|
| Balance | string | 是 |账户余额|
| TransferType | string | 是 | 交易类型	0001入金， 0002提现 |
