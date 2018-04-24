# 企业待收费列表

##### _【功能说明】_ {#【功能说明】}

企业待收费列表

_**【应用场景】**_

企业待收费列表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetParkFeeReportBySeller

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeTypeList |array int | 是 | 费用类型 |
| ParkSysNo| int | 否 | 园区编码|
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
| SellerName | string | 否 |企业名称 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ParkSysNo| int | 否 | 园区编码|
| ParkName | string | 否 | 园区名称|
| SellerMaster | string | 否 | 商家负责人|
| SellerTel | string | 否 | 联系电话|
| FeeDetails | array [FeeDetail] | 否 | 费用明细|

> #### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerCount | string | 否 | 商家数|
| ArrearsAmount | int | 是 | 欠费总金额  |
| FeeDetails | array [FeeDetail] | 否 | 费用明细|



###FeeDetail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeType| int | 否 |费用类型|
| ArrearsAmount | decimal | 否 |欠费金额 |











