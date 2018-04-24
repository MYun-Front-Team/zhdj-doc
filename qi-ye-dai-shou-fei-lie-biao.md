# 企业待收费列表

##### _【功能说明】_ {#【功能说明】}

企业待收费列表

_**【应用场景】**_

企业待收费列表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetParkFeeReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeTypeList |array int | 是 | 费用类型 |
| ParkSysNo| int | 否 | 园区编码|
| KeyWord| string| 否 | 关键字|


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







