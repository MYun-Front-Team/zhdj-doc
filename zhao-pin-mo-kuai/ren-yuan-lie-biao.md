# 人员列表

##### _【功能说明】_ {#【功能说明】}

人员列表

_**【应用场景】**_

人员列表

_**【接口地址】**_

[http://ip:port/RecruitAction/Customer/GetCustomerList](http://ip:port/RecruitAction/Customer/GetCustomerList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| KeyWord | string | 是 | 关键字 |
| AuthenticationStatus | int | 是 | 实名认证状态（0未认证 10已认证） |
| ContractStatus | int | 是 | 协议签署状态（0待签署10已经签署） |
| RecruitCertificateSysNo| int | 是 | 签约服务商编码 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| RealName | string | 是 | 人员姓名 |
| CellPhoneNo | string | 是 | 电话 |
| BankName | string | 是 | 开户行 |
| CardNo | string | 是 | 银行卡 |
| AuthenticationStatus | int | 是 | 实名认证状态（0未认证 10已认证） |
| ContractStatus | int | 是 | 协议签署状态（0待签署10已经签署） |
| ContractSysNo | int | 是 | 协议系统编码 |
| ContractSignTime | datetime | 是 | 协议签署时间 |
| NPLWalletCardNo | string | 是 | 电子钱包账号 |
| SellerName| string | 是 | 客户名称 |
| RecruitCertificateName| string | 是 | 签约主体 |










