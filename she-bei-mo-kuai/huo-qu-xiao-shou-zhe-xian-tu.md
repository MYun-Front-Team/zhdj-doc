# 获取销售月折线图 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetSaleMonthReport](http://ip:port/EqmQuery/Equipment/GetSaleReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LineSysNoList | array\[int\] | 否 | 路线数组 |

> #### _应答数据 \(数组\)_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Amount | decimal | 是 | 金额 |
| Date | datetime | 是 | 日期 |



