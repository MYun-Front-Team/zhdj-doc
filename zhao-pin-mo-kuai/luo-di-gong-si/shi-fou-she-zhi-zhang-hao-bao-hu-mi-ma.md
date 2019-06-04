# 检查保护密码是否正确

##### _【功能说明】_ {#【功能说明】}

检查保护密码是否正确


_**【应用场景】**_
检查保护密码是否正确



_**【接口地址】**_

http://ip:port/RecruitAction/MyBank/CheckPayPassword

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |
| RecruitCertificateSysNo| int| 是 | 落地公司编码 |
| PayPassword| string| 是 |保护密码 |



#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MyBankAccountStatus| int| 是 | 钱包账户状态，0无密码10密码正确11密码错误|




