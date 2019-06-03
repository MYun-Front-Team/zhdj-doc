# 获取商家落地公司列表
##### _【功能说明】_ {#【功能说明】}

获取商家落地公司列表


_**【应用场景】**_
获取商家落地公司列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Contract/GetSellerCertificateList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitServerSysNo| int | 否 | 服务商系统编码 |
| SellerSysNo| int | 否 | 商家系统编码 |



#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo| int | 是 | 主键 |
| SellerID| int | 是 | 商家编码 |
| SellerName| string| 是 | 商家名称 |
| RecruitCertificateName| string| 是 | 落地公司名称 |
| RecruitCertificateSysNo| int| 是 | 落地公司编码 |
| SubAccountNo| string| 是 | 子账号|
| PerMonthLimit| decimal| 是 | 每人单月限额 |
| ServerRate| decimal| 是 | 服务费比例 |
| RecruitServerSysNo| int | 是 | 服务商系统编码 |
| RecruitServerName| int | 是 | 服务商名称 |
