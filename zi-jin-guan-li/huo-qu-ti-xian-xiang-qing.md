# 获取提现详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取提现详情

_**【应用场景】**_

获取提现详情

_**【接口地址】**_

[http://ip:port/WalletQuery/ReceiveCash/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ReceiveCashBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReceiveCashSysNo | int | 是 | 提现系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReceiveCashSysNo | int | 是 | 提现系统编码 |
| Organization | object | 是 | 组织实体 |
| Wallet | object | 是 | 钱包实体 |
| ReceiveAmount | decimal（18，10） | 是 | 提现金额 |
| ReceiveStatus | int | 是 | 提现状态：0待处理，1已确认，10已提现，11已作废 |
| Card | object | 是 | 提现银行卡 |
| ReceiveTime | string | 是 | 提现时间 |
| ReceiveRemark | string | 否 | 提现申请说明 |
| DealRemark | string | 否 | 处理说明 |
| AuditPerson | object | 否 | 审核人实体 |
| AuditTime | string | 否 | 审核时间 |
| DealPerson | object | 否 | 处理人实体 |
| DealTime | string | 否 | 处理时间 |
| ReceiveCashType| int | 否 | 线上提现方式 0银行卡，1微信 |






