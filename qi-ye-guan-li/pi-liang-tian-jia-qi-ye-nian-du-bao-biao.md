# 批量添加企业年度报表

##### _【功能说明】_ {#【功能说明】}
批量添加企业年度报表

_**【应用场景】**_

批量添加企业年度报表
_**【接口地址】**_

http://ip:port/ParkAction/IndustrySale/ImportSaleYearReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|SaleYearReports|array[SaleYearReportImport]|企业年度报表|


> #### SaleYearReportImport

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerName | string | 是 | 商家名称 |
| Year | int| 是 |时间，只取年份  |
| TaxRevenue| decimal | 否 |预计年纳税额|
| Turnover | decimal | 否 |预计年销售额|




