# 绑定支付宝

##### _【功能说明】_ {#【功能说明】}

绑定支付宝

_**【应用场景】**_
绑定支付宝


_**【接口地址】**_

http://ip:port/RecruitAction/MyBank/BindAlipay

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo| string | 是 | 组织编码|
| PersonSysNo| int| 是 | 人员编码 |
| RecruitCertificateSysNo| int| 是 | 落地公司编码 |
| AccountNo| string| 是 | 支付宝账号 |
| AccountName| string| 是 | 支付宝对应的真实姓名|
| CertificateNo| string| 是 | 身份证号 |
| MobileNo| string| 否 | 预留手机号


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo| int | 是 | 银行卡编码 |



