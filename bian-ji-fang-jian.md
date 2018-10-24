# 添加房间

##### _【功能说明】_ {#【功能说明】}

添加房间

_**【应用场景】**_

添加房间

_**【接口地址】**_

http://ip:port/ParkAction/IndustryPark/EditParkRoom

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
|ParkRoomType | int | 否|房间类型|
| ParkRoomClassSysNo | int | 否 | 房间分类（枚举） |
| ParkFloorSysNo | int | 否 | 楼层系统编码 |
| ParkRoomName| int | 否 | 房间名称|
| FilePathList | array string | 否 |照片 |
| Remark | string | 否 |备注|
| ParkRoomAddress| string | 否 | 协议地址|
| BuildingArea| decimal | 否 |总建筑面积|
| Rent| decimal | 否 |租金单价|
| DrawingCode| string | 否 |图纸编码|
| IsPublic | int | 是 | 是否公共资源 |
| CalculateType| int | 是 |计价方式（1面积 2一口价） |
| ResourcesType| int | 是 |是否是不可用资源（0否 1是） |








> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



