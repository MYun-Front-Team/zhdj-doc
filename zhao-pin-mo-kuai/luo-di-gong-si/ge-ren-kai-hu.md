# 个人开户

##### _【功能说明】_ {#【功能说明】}

个人开户

_**【应用场景】**_

个人开户

_**【接口地址】**_

http://ip:port/RecruitQuery/MyBank/PersonalRegister

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName | string | 是 | 人员姓名 |
| IDCard | string | 是 | 身份证号 |
| CardNo | string | 是 | 银行卡号 |
| BankSysNo | int | 否 | 银行编码 |
| BankName | string | 是 | 银行名称 |
| BankBranchName | string | 是 | 支行名称 |



#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberID | string| 是 | 网上银行会员号 |
| SubAccountNo |string | 是 | 子账号 |



