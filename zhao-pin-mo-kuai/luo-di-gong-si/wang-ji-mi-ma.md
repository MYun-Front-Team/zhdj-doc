# 忘记密码

##### _【功能说明】_ {#【功能说明】}

忘记密码

_**【应用场景】**_
忘记密码



_**【接口地址】**_

http://ip:port/RecruitAction/MyBank/ResetPayPassword

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |
| RecruitCertificateSysNo| int| 是 | 落地公司编码 |
| MemberID| string| 是 |网商银行会员号 |
| Captcha| string| 是 |验证码|
| NewPayPassword| string| 是 |新保护密码 |


#### 返回参数

无



