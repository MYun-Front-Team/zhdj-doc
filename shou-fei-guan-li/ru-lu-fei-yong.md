# 入录费用

##### _【功能说明】_ {#【功能说明】}

入录费用

_**【应用场景】**_

入录费用

_**【接口地址】**_

http://ip:port/ParkAction/IndustryFee/AddFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeType | int | 是 | 费用类型 |
| FeeClassSysNo | int | 否 | 费用分类（枚举） |
| StartDate | datetime | 是 | 费用开始时间 |
| EndDate | datetime | 是 | 费用结束时间 |
| ParkSysNo| int | 是 | 园区编码|
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| Remark | string| 否 | 备注|
| AddFeeItems | array[AddFeeItem] | 否 | 导入明细|
| DiscountAmonut| decimal | 否 |折扣费用|
| IncreaseAmonut| decimal | 否 |加收费用|




 #### AddFeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BuildingName | string | 是  | 楼宇名称 |
| ParkRoomName| string | 是  | 房间名称|
|ParkRoomType | int | 是 |房间类型|
| FeeItemType| int | 是  |费用类型（端定义）|
| UnitFee| decimal | 是  |单价|
| Count| decimal | 是  |数量（支持小数点）|
| TotalFee| decimal | 是  |总价（非计算，按照客户填的为准）|
| ItemStartDate| datetime | 否 |开始日期|
| ItemEndDate| datetime | 否 |截止日期|
| ParkName | string | 否 | 园区名称 |
| ParkFloorName | string | 否 | 楼层名称 |
| BuildingArea| decimal | 否 |总建筑面积|
| CalculateType| int | 否 |计价方式（1面积 2一口价） |
| ParkRoomSysNo | int | 是 | 房间系统编码 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeSysNo | int | 是 | 费用系统编码 |









