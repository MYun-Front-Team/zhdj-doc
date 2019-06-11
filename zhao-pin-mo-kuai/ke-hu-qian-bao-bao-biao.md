# 客户钱包报表

##### _【功能说明】_ {#【功能说明】}

客户钱包报表

_**【应用场景】**_

客户钱包报表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Wallet/GetWalletReport](http://ip:port/RecruitQuery/Wallet/GetWalletReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeAmount | decimal（18，2） | 是 | 实发金额 |
| ServerAmount | decimal（18，2） | 是 | 服务费 |
| TotalAmount | decimal（18，2） | 是 | 账户总余额 |
| PaidCount | int | 是 | 发放笔数 |
| FinishAmount | decimal（18，2） | 是 | 成功发放金额 |
| GoingAmount | decimal（18，2） | 是 | 发放中金额 |
| Items| array[WalletReportItem] | 是 | 发放中金额 |



> #### 应答数据 WalletReportItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeAmount | decimal（18，2） | 是 | 实发金额 |
| RecruitCertificateName| string | 是 | 落地公司名称 |
| RecruitCertificateSysNo| int | 是 | 落地公司编码|


