# 获取充值详情

##### _【功能说明】_ {#【功能说明】}

获取充值详情

_**【应用场景】**_

获取充值详情

_**【接口地址】**_

http://ip:port/RecruitQuery/Wallet/GetRechargeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值编码 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| RechargeAmount | decimal（18，2） | 是 | 充值金额 |
| Remark | string | 否 | 备注 |
| FilePathList |array[string] | 否 |凭证 |
| ServerRate| decimal（18，2） | 是 | 服务费比率（0～1）|
| ServerAmount| decimal（18，2） | 是 | 服务费|
| SellerName | string | 是 | 商家名称 |
| RechargeStatus | int | 是 | 0待审核，10成功，11失败|

