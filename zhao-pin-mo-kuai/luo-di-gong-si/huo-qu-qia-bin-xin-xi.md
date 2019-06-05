# 获取卡BIN信息

##### _【功能说明】_ {#【功能说明】}

获取卡BIN信息


_**【应用场景】**_
获取卡BIN信息


_**【接口地址】**_

http://ip:port/RecruitQuery/MyBank/GetCardBin

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo| string| 是 | 银行卡号 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardBin| string| 是 | 卡BIN信息|
| CardType| string| 是 | 卡类型，DC: 借 记 卡, CC: 贷 记卡,SCC:准贷记卡|
| BranchNo| string| 是 | 机构联行号|
| BankName| string| 是 | 所属银行名称|












