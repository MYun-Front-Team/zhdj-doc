# 费用导入

##### _【功能说明】_ {#【功能说明】}

Excel导入，按同园区同企业group by成一条记录

_**【应用场景】**_

费用导入

_**【接口地址】**_

http://ip:port/ParkAction/IndustryFee/ImportFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| ImportFeeItems | array[ImportFeeItem] | 否 | 导入明细|

 #### ImportFeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkName | string | 是 | 园区名称|
| BuildingName | string | 是  | 楼宇名称 |
| SellerName | string | 是  |企业名称 |
| ParkRoomName| string | 是  | 房间名称|
|ParkRoomType | int | 是 |房间类型|
| FeeItemType| int | 是  |费用类型（端定义）|
| UnitFee| decimal | 是  |单价|
| Count| decimal | 是  |数量（支持小数点）|
| TotalFee| decimal | 是  |总价（非计算，按照客户填的为准）|
| ItemStartDate| datetime | 否 |开始日期|
| ItemEndDate| datetime | 否 |截止日期|












