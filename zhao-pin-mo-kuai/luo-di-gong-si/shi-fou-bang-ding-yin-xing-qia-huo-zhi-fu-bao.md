# 是否绑定银行卡或支付宝

##### _【功能说明】_ {#【功能说明】}

是否绑定银行卡或支付宝

_**【应用场景】**_
是否绑定银行卡或支付宝


_**【接口地址】**_

http://ip:port/RecruitQuery/MyBank/CheckBindCardOrAlipay

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |
| RecruitCertificateSysNo| int| 是 | 落地公司编码 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsBindCard| int | 是 | 是否绑定，0未绑定1已绑定 |
| IsBindAlipay| int | 是 | 是否绑定，0未绑定1已绑定 |


