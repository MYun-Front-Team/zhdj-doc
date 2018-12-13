# 获取钱包排行榜

##### _【功能说明】_ {#【功能说明】}

获取钱包排行榜

_**【应用场景】**_

获取钱包排行榜


_**【接口地址】**_


http://ip:port/WalletQuery/Wallet/GetLJWalletRank

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string| 是 | 买家人员昵称 |
| HisAmount| decimal| 是 | 历史资金|
| FileUrlList | array string | 否 | 头像图片列表 |

