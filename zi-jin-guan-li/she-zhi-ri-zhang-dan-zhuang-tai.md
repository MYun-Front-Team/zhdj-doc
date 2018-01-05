# 设置日账单状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置日账单状态

_**【应用场景】**_

设置日账单状态

注：记录日账单的处理人和处理时间；

_**【接口地址】**_

[http://ip:port/WalletAction/DailyBill/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etDailyBillStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DailyBillSysNo | int | 是 | 日账单系统编码 |
| BillDealStatus | int | 是 | 账单处理状态：0待处理，10已处理，11已作废 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



