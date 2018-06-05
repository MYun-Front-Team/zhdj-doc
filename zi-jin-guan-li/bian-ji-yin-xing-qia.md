# 编辑银行卡

##### _【功能说明】_ {#【功能说明】}

编辑银行卡

_**【应用场景】**_

编辑银行卡

_**【接口地址】**_

http://ip:port/WalletAction/Card/EditCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo | int | 是 | 系统编码 |
| CardType | int | 是 | 银行卡类型：0普通，1信用卡 |
| CardNo | string | 是 | 银行卡号 |
| CardName | string | 是 | 银行卡户名 |
| CardPhoneNo | string | 是 | 预留手机号 |
| BankSysNo | int | 是 | 银行系统编码 |
| BankBranchName | string | 是 | 开户行-支行名称 |
| PCDCode | string | 否 | PCD编码 |
| PCDDescription | string | 否 | PCD详情 |
| AccountAddress | string | 否 | 开户行地址 |
| CardKey | string | 否 | 信用卡口令 |
| CardDate | string | 否 | 信用卡有效期 |




