# 充值 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

充值

_**【应用场景】**_

充值

注：只有激活状态的卡，才能充值；

把充值金额充值到组织钱包，并记录日志；

_**【接口地址】**_

[http://ip:port/WalletAction/MemberCard/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddMemberCardAmount

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo | string | 是 | 卡号 |
| CardAmount | decimal（18，2） | 是 | 金额 |
| GiveAmount | decimal（18，2） | 否 | 赠送金额 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值系统编码 |



