# 重点企业销售额统计表

##### _【功能说明】_ {#【功能说明】}

重点企业销售额统计表

_**【应用场景】**_

重点企业销售额统计表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetTurnoverReportBySeller

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ScaleTypeList |array int | 是 |规模（端定义）|
| Year | int| 否 |时间，只取年份  |
| KeyWord| string| 否 | 关键字|
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ParkSysNo| int | 否 | 园区编码|



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Items | array[object] | 是 | 基础字段 |
| Total | object | 否 | 统计字段 |

> #### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Year | int| 否 |时间，只取年份  |
| ParkName | string | 否 | 园区名称|
| SellerName | string | 否 |企业名称 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| OfficeBuildingArea| decimal | 否 |办公总面积|
| RegistrationTime| datetime| 否 |注册时间 |
| InitialTurnover | decimal | 否 |初始销售额|
| Turnover | decimal | 否 |最终销售额|
| FeeDetails | array [FeeDetail] | 否 | 费用明细|

> #### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  InitialTurnover | decimal | 否 |初始销售额|
| Turnover | decimal | 否 |最终销售额|
| FeeDetails | array [FeeDetail] | 否 | 费用明细|



###FeeDetail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Month| int | 否 |费用类型|
| Turnover | decimal | 否 |最终销售额|












