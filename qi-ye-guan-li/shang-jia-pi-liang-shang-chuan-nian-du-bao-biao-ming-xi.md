# 商家上传年度报表明细

##### _【功能说明】_ {#【功能说明】}
商家上传年度报表明细（遍历月份明细，如果如果数据库当前月份已经存在，则更新，不存在则新增，如果商家该年份的主表记录不存在，则提醒需要先添加企业年度报表）
_**【应用场景】**_

商家上传年度报表明细（遍历月份明细，如果数据库当前月份已经存在，则更新，不存在则新增，如果商家该年份的主表记录不存在，则提醒需要先添加企业年度报表）


_**【接口地址】**_

http://ip:port/ParkAction/IndustrySale/ImportSaleYearReportDetail

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|SaleYearReportDetails|array[SaleYearReportDetailImport]|企业年度报表|




> #### SaleYearReportDetailImport

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerName | string | 是 | 商家名称 |
| Year | int| 是 |时间，只取年份  |
| Items| array[SaleYearReportDetailImportItem]| 是 |费用信息 |


> #### SaleYearReportDetailImportItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InitialTaxRevenue| decimal | 否 |企业上报税额|
| InitialTurnover| decimal | 否 |企业上报销售额|
| TaxRevenue| decimal | 否 |平台实际税额|
| Turnover | decimal | 否 |平台实际销售额|
| TotalTaxRevenue| decimal | 否 |本年累计税额|
| TotalTurnover | decimal | 否 |本年累计销售额|
| Month| int | 是 | 月份 |














