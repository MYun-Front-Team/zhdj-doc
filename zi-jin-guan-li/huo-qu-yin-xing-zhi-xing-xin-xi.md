# 获取银行支行信息

##### _【功能说明】_ {#【功能说明】}

获取银行支行信息

_**【应用场景】**_

获取银行支行信息

_**【接口地址】**_

http://ip:port/WalletQuery/Bank/GetBankBranchList

> #### _请求数据_ {#请求数据}

| 参数名 | 类型 | 是否必须 | 说明 |
| :--- | :--- | :--- | :--- |
| CardNo | string | 是 | 银行卡号 |
| BankName | string | 是 | 银行名称 |
| Province | string | 否 | 省 |
| City | string | 否 | 市 |
| District | string | 否 | 区 |
| Step | int | 是 | 步骤（1为第一步，2为第二步） |
| Page | int | 是 | 请求页码，从1开始 |

### 应答参数\(数组\) {#请求参数改动}

| 参数名 | 类型 | 是否必须 | 说明 |
| :--- | :--- | :--- | :--- |
| province | string | 是 | 省 |
| city | string | 是 | 是 |
| district | string | 是 | 区 |
| street | string | 是 | 街道 |
| address | string | 是 | 地址 |
| bankname | string | 是 | 银行名称 |
| branchname | string | 是 | 支行名称 |
| number | string | 是 | 联行号 |
| phone | string | 是 | 电话 |
| lng | string | 是 | 经度 |
| lat | string | 是 | 纬度 |































