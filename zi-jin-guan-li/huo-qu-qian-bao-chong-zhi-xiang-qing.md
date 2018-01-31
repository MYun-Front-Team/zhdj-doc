# 获取钱包充值详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取钱包充值详情

_**【应用场景】**_

获取钱包充值详情

_**【接口地址】**_

[http://ip:port/WalletQuery/Wallet/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RechargeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 钱包充值系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 钱包充值系统编码 |
| RechargeStatus | int | 是 | 状态：0初始化， 10已完成，11已删除 |
| RechargeAmount | decimal（18，10） | 是 | 充值金额 |
| PaymentAmount | decimal（18，10） | 是 | 实际支付金额 |
| GiveAmount | decimal（18，10） | 是 | 赠送金额 |
| Remark | string | 否 | 备注 |



