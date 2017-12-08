# 确认提现 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

确认提现

_**【应用场景】**_

确认提现

注：1、判断钱包余额是否充足，满足则减少钱包余额，记录钱包log日志；

2、记录通用log日志，确认人信息；

3、需防并发或者重复点击事件，需加锁；

_**【接口地址】**_

[http://ip:port/WalletAction/ReceiveCash/F](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)inishReceiveCash

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReceiveCashSysNo | int | 是 | 提现系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



