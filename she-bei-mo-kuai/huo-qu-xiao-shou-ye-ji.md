# 获取销售业绩 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetSaleReport](http://ip:port/EqmQuery/Equipment/GetSaleReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LineSysNoList | array\[int\] | 否 | 路线数组 |
| StartTime | datetime | 否 | 开始时间 |
| EndTime | datetime | 否 | 结束时间 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Amount | decimal | 是 | 金额 |
| Online | decimal | 是 | 移动 |
| Cash | decimal | 是 | 现金 |
| YestAmount | decimal | 是 | 昨日金额 |
| YestOnline | decimal | 是 | 昨日移动 |
| YestCash | decimal | 是 | 昨日现金 |
| MonAmount | decimal | 是 | 本月金额 |
| MonOnline | decimal | 是 | 本月移动 |
| MonCash | decimal | 是 | 本月现金 |
| LastMonAmount | decimal | 是 | 上月金额 |
| LastMonOnline | decimal | 是 | 上月移动 |
| LastMonCash | decimal | 是 | 上月现金 |



