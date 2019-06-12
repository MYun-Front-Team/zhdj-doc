# 查询余额

##### _【功能说明】_ {#【功能说明】}

查询余额


_**【应用场景】**_
查询余额


_**【接口地址】**_

http://ip:port/RecruitQuery/MyBank/GetBalance

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AvailableBalance| decimal| 是 |可用余额|
| Balance| decimal| 是 |余额|
| AccountList| array[MyBankAccount]| 是 | 账户列表|

#### 返回参数MyBankAccount

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AvailableBalance| decimal| 是 |可用余额|
| Balance| decimal| 是 |余额|
| AccountID| string| 是 | 账户ID|
| AccountType| string| 是 | 账户类型|
| SubAccountNo| string| 是 | 子账户|









