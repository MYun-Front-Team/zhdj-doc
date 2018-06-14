# 提示信息报表

##### _【功能说明】_ {#【功能说明】}

提示信息报表

_**【应用场景】**_
提示信息报表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetFeeTipInfo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 企业组织系统编码 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeTipTotal | FeeTipTotal | 是 | 汇总信息 |
| FeeTipItems | array[FeeTipItem] | 否 |欠费 |




> #### FeeTipItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeType | int | 是 | 费用类型 |
| TotalFee | decimal | 否 |欠费 |



> #### FeeTipTotal

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerCount | int| 否 |未缴费商家数|
| Deposit | decimal | 否 | 押金 |













