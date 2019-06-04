# 绑定银行卡

##### _【功能说明】_ {#【功能说明】}

绑定银行卡

_**【应用场景】**_
绑定银行卡


_**【接口地址】**_

http://ip:port/RecruitAction/MyBank/BindCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |
| CardNo| string| 是 | 银行卡 |
| BankName| string| 是 | 银行全称 |
| AccountName| string| 是 | 银行开户名 |
| CardType| string| 是 | 卡类型，DC借记CC贷记（信用卡）PB存折OC其他|
| CardAttribute| string| 是 | 卡属性，C对私B对公 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo| int | 是 | 银行卡编码 |



