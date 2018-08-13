# 福狸获取资金信息

##### _【功能说明】_ {#【功能说明】}

福狸获取资金信息

_**【应用场景】**_

福狸获取资金信息

_**【接口地址】**_

http://ip:port/WalletQuery/Wallet/GetFLWallet

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| PersonSysNo| int | 是 | 人员系统编码 |
| StartDate| string | 是 | 开始时间 |
| EndDate| string | 是 | 结束时间 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 否 | 佣金信息 |
| Items| List[Item]| 否 | 每日粉丝情况信息 |






> #### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Commission| decimal | 否 | 效果预估佣金 |
| FinishCommission| decimal（18，10） | 是 | 结算效果预估 |
| SaveAmount| decimal（18，10） | 是 |节省金额 |


> #### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewFans| int| 否 | 新增粉丝数 |
| FansOrderCount|int| 是 | 粉丝下单数 |
| FansOrderAmount|decimal| 是 | 粉丝下单金额 |
| Date| string | 是 | 时间 |
| Commission| decimal | 否 | 效果预估佣金 |





