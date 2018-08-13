# 获取企业租赁房间列表

##### _【功能说明】_ {#【功能说明】}
获取企业租赁房间列表

_**【应用场景】**_

获取企业租赁房间列表

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetParkRoomRentList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| IfShowRent| int | 否 | 是否只显示当前租的|
| ParkRoomSysNo| int | 否 | 房间编码|






> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomRentSysNo | int | 是 | 租赁系统编码 |
| StartDate | datetime| 是 | 入住时间 |
| EndDate | datetime| 是 | 退租时间 |
| Remark | string | 是 | 租赁备注 |
| ParkRoomSysNo| int | 否 | 房间编码|
| ParkRoomName| string | 否 | 房间名称|
| ParkFloorName | string | 否 | 楼层名称 |
| ParkName | string | 否 | 园区名称|
| BuildingName | string | 否 | 楼宇名称 |
|ParkRoomType | int | 是 |房间类型|
| BuildingArea| decimal | 否 |总建筑面积|
| Rent| decimal | 否 |租金单价|
| SellerName | string | 是 | 商家名称 |
| FeeEndDate | datetime | 否 | 费用结束时间 |









