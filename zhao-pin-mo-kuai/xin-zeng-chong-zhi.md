# 新增充值

##### _【功能说明】_ {#【功能说明】}

新增充值

_**【应用场景】**_

新增充值

_**【接口地址】**_

[http://ip:port/RecruitAction/Wallet/AddRecharge](http://ip:port/RecruitAction/Wallet/AddRecharge)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| RechargeAmount | decimal（18，2） | 是 | 充值金额 |
| FilePathList | array\[string\] | 否 | 凭证 |
| RecruitCertificateSysNo| int| 是 |签约服务商编码 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值编码 |



