# 批量编辑企业年度报表明细

##### _【功能说明】_ {#【功能说明】}
平台获取年度报表明细

_**【应用场景】**_

平台获取年度报表明细

_**【接口地址】**_

http://ip:port/ParkAction/IndustrySale/EditSaleYearReportDetails

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportSysNo| int | 是 | 年度报表系统编码 |
| SaleYearReportDetails|array[SaleYearReportDetailEdit]| 是 | 年度报表明细 |


> #### SaleYearReportDetailEdit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportItemSysNo | int | 是 | 年度报表明细系统编码 |
| TaxRevenue| decimal | 否 |最终税额|
| Turnover | decimal | 否 |最终销售额|
| TotalTaxRevenue| decimal | 否 |本年累计税额|
| TotalTurnover | decimal | 否 |本年累计销售额|
| InitialTaxRevenue| decimal | 否 |企业上报税额|
| InitialTurnover| decimal | 否 |企业上报销售额|


