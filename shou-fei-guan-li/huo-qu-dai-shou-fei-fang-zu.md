# 新增待收费查询

##### _【功能说明】_ {#【功能说明】}

新增待收费查询（只对房租和物业费有效）

_**【应用场景】**_

新增待收费查询（只对房租和物业费有效）



_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetWaitPayFee



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeType | int | 是 | 费用类型 |
| EndDate | datetime | 是 | 费用结束时间 |
| ParkFloorSysNo | int | 否 | 楼层编码 |
| ParkSysNo | int | 否 | 园区编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
|ParkRoomType | int | 否 |房间类型|
| StartDateInfos| array[StartDateInfo]| 否 | 费用开始时间 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WaitPayFeeItems| array[WaitPayFeeItem]| 否 | 费用明细 |
| WaitPayFeeTotal| WaitPayFeeTotal| 否 | 费用汇总 |

#### StartDateInfo

| 变量名 | 类型 | 是否必须 | 描述 |
|ParkRoomSysNo | int | 是 |房间系统编码|
| StartDate| datetime | 是 |费用开始时间|

> #### WaitPayFeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkFloorSysNo | int | 否 | 楼层编码 |
| ParkSysNo | int | 否 | 园区编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ParkName | string | 否 | 园区名称 |
| ParkRoomName| int | 否 | 房间名称|
| ParkFloorName | string | 否 | 楼层名称 |
| BuildingName | string | 否 | 楼宇名称 |
|ParkRoomType | int | 是 |房间类型|
| Rent| decimal | 否 |费用单价|
| BuildingArea| decimal | 否 |总建筑面积|
| CalculateType| int | 是 |计价方式（1面积 2一口价） |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| TotalMonth| decimal| 否 | 月份 |
| TotalRent| decimal| 否 | 总费用|

> #### WaitPayFeeTotal

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalRent| decimal| 否 | 总费用|



