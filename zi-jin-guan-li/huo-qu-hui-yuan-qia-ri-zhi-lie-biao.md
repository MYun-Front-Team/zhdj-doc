# 获取会员卡日志列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取会员卡日志列表

_**【应用场景】**_

获取会员卡日志列表

_**【接口地址】**_

[http://ip:port/WalletQuery/MemberCard/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMemberCardLogList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartTime | string | 否 | 开始时间 |
| EndTime | string | 否 | 结束时间 |
| KeyWord | string | 否 | 身份证/手机号/卡号 |
| CardStatusList | int | 否 | 日志类型：1开卡，2挂失，3退卡，4充值 |
| IsShowStatistics | int | 否 | 是否显示统计数据 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardLogList | array object | 是 | 日志 |
| MemberCardStatistics | array object | 是 | 统计 |

#### MemberCardLog说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardLogSysNo | int | 是 | 会员卡系统编码 |
| Card | object | 否 | 会员卡（实时数据） |
| CardNo | string | 是 | 卡号（冗余） |
| CardPhoneNo | string | 否 | 手机号（冗余） |
| IDCard | string | 否 | 身份证（冗余） |
| CardAmount | decimal（18，2） | 是 | 金额 |
| CardStatus | int | 否 | 日志类型：1开卡，2挂失，3退卡，4充值 |
| Person | object | 是 | 操作人 |
| CreateTime | string | 是 | 操作时间 |
| GiveAmount | decimal（18，2） | 否 | 其中赠送金额 |
| PaymentType | int | 否 | 支付方式 |
| Remark | string | 否 | 备注 |
| CardType | int | 否 | 会员卡类型 |

#### MemberCardStatistic说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡 |
| CardCount | int | 是 | 数量 |



