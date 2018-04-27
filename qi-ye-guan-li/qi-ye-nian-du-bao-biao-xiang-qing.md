# 企业年度报表详情

##### _【功能说明】_ {#【功能说明】}
企业年度报表详情

_**【应用场景】**_

企业年度报表详情

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetSaleYearReportBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportSysNo | int | 是 | 年度报表系统编码 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportSysNo | int | 是 | 年度报表系统编码 |
| Year | int| 是 |时间，只取年份  |
| TaxRevenue| decimal | 否 |预计年纳税额|
|  Turnover | decimal | 否 |预计年销售额|







