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
| IDCard | string| 是 |身份证号|
| Captcha| string| 否 |验证码，重置新密码时必传|
| NewPayPassword| string| 否 |新保护密码，重置新密码时必传 |


#### 返回参数

无



