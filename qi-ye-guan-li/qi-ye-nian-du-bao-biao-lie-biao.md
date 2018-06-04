# 企业年度报表列表

##### _【功能说明】_ {#【功能说明】}
企业年度报表列表

_**【应用场景】**_

企业年度报表列表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetSaleYearReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 企业组织系统编码 |
| Year | int | 否 |时间，只取年份 |
| ParkSysNo| int | 否 |注册地址（园区） |
|InParkStatusList|array[int] | 否 |状态（潜在客户，已入驻，已签出） |
| SellerClassSysNo | int | 否 | 商家类别系统编码（类目树） |
|KeyWord|string| 否 |关键字 |





> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportSysNo | int | 是 | 年度报表系统编码 |
| Year | int| 是 |时间，只取年份  |
| TaxRevenue| decimal | 否 |预计年纳税额|
|  Turnover | decimal | 否 |预计年销售额|
| TotalTaxRevenue| decimal | 否 |年纳税额|
|  TotalTurnover | decimal | 否 |年销售额|
| SellerName | string | 是 | 商家名称 |
| SellerTel | string | 否 | 商家联系电话 |
| SellerMaster | string | 否 | 商家负责人 |














