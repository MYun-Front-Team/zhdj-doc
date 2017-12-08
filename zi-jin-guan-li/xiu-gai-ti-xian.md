# 新增提现 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增提现

_**【应用场景】**_

新增提现

注：记录log日志；

1、需判断可用余额是否充足；（冻结金额是修改前金额，如果改大提现金额，需二者作差来判断可用余额是否充足）

_**【接口地址】**_

[http://ip:port/WalletAction/ReceiveCash/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditReceiveCash

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReceiveCashSysNo | int | 是 | 提现系统编码 |
| ReceiveAmount | decimal（18，10） | 否 | 提现金额 |
| CardSysNo | int | 否 | 提现银行卡系统编码 |
| ReceiveTime | string | 否 | 提现时间 |
| ReceiveRemark | string | 否 | 提现申请说明 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



