# 平台基础数据报表

##### _【功能说明】_ {#【功能说明】}

平台基础数据报表

_**【应用场景】**_

平台基础数据报表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Wallet/GetPlatWalletReport](http://ip:port/RecruitQuery/Wallet/GetPlatWalletReport)

> #### _请求数据_ {#请求数据}

无

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalAmount | decimal（18，2） | 是 | 总发放金额 |
| TotalCount | decimal（18，2） | 是 | 总发放笔数|
| CustomerTotalCount | long | 是 | 客户总数 |
| PlatTotalAmount | decimal（18，2） | 是 | 平台总流水 |



