# 添加落地公司
##### _【功能说明】_ {#【功能说明】}

添加落地公司


_**【应用场景】**_

添加落地公司


_**【接口地址】**_

http://ip:port/RecruitAction/Contract/AddCertificate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitCertificateSysNo| int | 是 | 落地公司系统编码 |
| SellerSysNo| int | 是 |商家系统编码 |
| PerMonthLimit| decimal | 是 |每人单月限额 |
| ServerRate| decimal | 是 |服务费比例|




#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo| int | 是 | 商家下的落地公司系统编码 |