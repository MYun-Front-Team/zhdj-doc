# 获取银行支行信息
##### _【功能说明】_ {#【功能说明】}

获取银行支行信息

_**【应用场景】**_

获取银行支行信息

_**【接口地址】**_
http://ip:port/WalletQuery/Bank/GetBankBranchList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo| string | 是 | 银行卡系统编码 |
| BankName | string | 是 | 银行名称 |
| Province| string | 否 | 省|
| City| string | 否 | 市|
| District| string | 否 | 区|
| Step| int| 否 | Step|
| Page| int| 否 | Page|






