# 获取合同列表
##### _【功能说明】_ {#【功能说明】}

获取合同列表


_**【应用场景】**_

获取合同列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Contract/GetCertificateList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitServerSysNo| int | 否 | 服务商系统编码 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CertificateSysNo| int | 是 | 证书系统编码 |
| SellerName| string| 是 | 签约主体 |
| ContractAddress| string| 是 | 地址 |
| ZipCode| string| 是 | 邮编 |
| CreditCode| string| 是 | 信用代码 |
| SellerMaster| string| 是 | 法人代表名称 |
| SellerIDCard| string| 是 | 法人代表证件号 |
| SellerMasterPhone| string| 是 | 法人代表电话 |
| CertificateStatus| int | 是 | 证书申请状态（10通过） |
| TemCount| int | 是 | 模板数量|
| RecruitServerSysNo| int | 是 | 服务商系统编码 |
| RecruitServerName| int | 是 | 服务商名称 |
