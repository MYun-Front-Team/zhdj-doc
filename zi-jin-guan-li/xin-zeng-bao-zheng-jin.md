# 新增保证金 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增保证金

_**【应用场景】**_

新增保证金

_**【接口地址】**_

[http://ip:port/WalletAction/Wallet/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddBond

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| PaidAmount | decimal（18，2） | 是 | 缴费费用 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BondSysNo | int | 是 | 系统编码 |



