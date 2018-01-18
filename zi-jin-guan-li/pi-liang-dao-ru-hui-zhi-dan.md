# 批量导入回执单 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

批量导入回执单

_**【应用场景】**_

批量导入回执单

注：1、根据“账单日”和“卡号”、“金额”，验证是否存在这样一条合法的提现申请；（不合法就提示）

2、验证通过后，把对应的提现记录标记已处理，处理人，处理时间，处理备注；

3、全部完成后，重新统计这笔日账单是否已全部结算；

4、记录日账单的审核人和审核时间；

_**【接口地址】**_

[http://ip:port/WalletAction/DailyBill/Import](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DailyBillReceipt

> #### _请求数据（DailyBillReceipts数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BillDate | string | 是 | 账单日 |
| CardNo | string | 是 | 银行卡号 |
| CardName | string | 是 | 银行卡户名 |
| BankBranchName | string | 是 | 开户行-支行名称 |
| Amount | decimal（18，2） | 是 | 金额 |
| DealRemark | string | 否 | 处理说明 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



