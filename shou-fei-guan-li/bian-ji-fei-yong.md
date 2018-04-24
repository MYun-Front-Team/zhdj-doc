# 入录费用

##### _【功能说明】_ {#【功能说明】}

入录费用

_**【应用场景】**_

入录费用

_**【接口地址】**_

http://ip:port/ParkAction/IndustryFee/EditFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeSysNo | int | 是 | 费用系统编码 |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| ParkSysNo| int | 否 | 园区编码|
| OrganizationSysNo | int | 否 | 企业组织系统编码 |
| Remark | int | 否 | 备注|
| ParkSysNo| int | 否 | 园区编码|
| EditFeeItems | array[EditFeeItem] | 否 | 导入明细|

 #### EditFeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeItemSysNo | int | 是 |费用明细编码 |
| BuildingName | string | 否  | 楼宇名称 |
| ParkRoomName| string | 否  | 房间名称|
|ParkRoomType | int | 否 |房间类型|
| FeeItemType| int | 否 |费用类型（端定义）|
| UnitFee| decimal | 否 |单价|
| Count| decimal | 否 |数量（支持小数点）|
| TotalFee| decimal | 否 |总价（非计算，按照客户填的为准）|
| ItemStartDate| datetime | 否 |开始日期|
| ItemEndDate| datetime | 否 |截止日期|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |










