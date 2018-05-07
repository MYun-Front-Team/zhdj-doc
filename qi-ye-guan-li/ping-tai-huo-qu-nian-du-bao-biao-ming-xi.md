# 平台获取年度报表明细

##### _【功能说明】_ {#【功能说明】}
平台获取年度报表明细

_**【应用场景】**_

平台获取年度报表明细

_**【接口地址】**_

http://ip:port/ParkAction/IndustrySale/EditSaleYearReportDetail

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| YearReportItemSysNo | int | 是 | 年度报表明细系统编码 |
| TaxRevenue| decimal | 否 |最终税额|
| Turnover | decimal | 否 |最终销售额|
| TotalTaxRevenue| decimal | 否 |本年累计税额|
| TotalTurnover | decimal | 否 |本年累计销售额|
| FilePathList | array string | 否 |照片 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |









