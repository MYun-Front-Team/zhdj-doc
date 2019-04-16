# 递交实名认证

##### _【功能说明】_ {#【功能说明】}

递交实名认证

_**【应用场景】**_

递交实名认证

_**【接口地址】**_

[http://ip:port/RecruitQuery/Authentication/SubmitAuthentication](http://ip:port/RecruitQuery/Authentication/SubmitAuthentication)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName | string | 是 | 人员姓名 |
| CardNo | string | 是 | 银行卡号 |
| BankSysNo | int | 否 | 银行编码 |
| BankName | string | 是 | 银行名称 |
| BankBranchName | string | 是 | 支行名称 |
| IDCard | string | 是 | 身份证号 |
| OriginAddress | string | 是 | 户籍地址 |
| ContractAddress | string | 是 | 联系地址 |
| ZipCode | string | 是 | 邮编 |
| FPersonIDCardUrl | string | 否 | 身份证正面 |
| BPersonIDCardUrl | string | 否 | 身份证反面 |
| CellPhoneNo | string | 否 | 银行预留手机号 |
| Captcha | string | 否 | 验证码 |
| Uuid | string | 否| 验证码流水号 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuthenticationSysNo | int | 是 | 实名认证系统编码 |



