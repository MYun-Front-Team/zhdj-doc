# 获取日账单详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取日账单详情

_**【应用场景】**_

获取日账单详情

_**【接口地址】**_

[http://ip:port/WalletQuery/DailyBill/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DailyBillBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DailyBillSysNo | int | 是 | 日账单系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DailyBill | object | 是 | 日账单 |
| ReceiveCashList | array object | 是 | 提现记录列表 |



