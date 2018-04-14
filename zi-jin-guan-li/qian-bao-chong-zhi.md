# 钱包充值

##### _【功能说明】_ {#【功能说明】}

钱包充值

_**【应用场景】**_

钱包充值

_**【接口地址】**_

http://ip:port/WalletAction/Wallet/AddWallet

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| RechargeAmount | decimal（18，2） | 是 | 充值金额 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值编码 |



