# 获取发放列表

##### _【功能说明】_ {#【功能说明】}

获取发放列表

_**【应用场景】**_

获取发放列表

_**【接口地址】**_

http://ip:port/RecruitAction/Wallet/GetWageList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| WageStatusList | array[int] | 是 | 单据状态（0待发 1发放中，10已发放）|
| KeyWord | string | 是 | 关键字 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WageSysNo | int | 是 | 发放编码 |
| OrganizationSysNo | int | 是 | 组织系统编码  |
| SellerName | string | 是 | 商家名称 |
| WageAmount | deimal | 是 | 实发金额|
| ServerAmount | deimal | 是 | 服务费金额|
| SuccessCount | int | 是 | 成功数量 |
| FailCount | int | 是 | 失败数量 |
| WageStatus | int | 是 | 单据状态（0待发 1发放中，10已发放）|




