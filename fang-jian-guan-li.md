# 房间管理

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
| ParkFloorSysNo | int |是 | 楼层编码 |
| ParkFloorName| string|是 | 楼层名称 |
| BuildingSysNo | int | 是 | 楼宇编码 |
| BuildingName| int | 是 | 楼宇名称  |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
|ParkRoomType | int | 是 |房间类型|
| ParkRoomClassSysNo | int | 否 | 房间分类（枚举） |
| ParkRoomName| int | 否 | 房间名称|
| FilePathList | array string | 否 |照片 |
| Remark | string | 否 |备注|
| ParkRoomAddress| string | 否 | 协议地址|
| BuildingArea| decimal | 否 |总建筑面积|
| Rent| decimal | 否 |租金单价|
| DrawingCode| string | 否 |图纸编码|
| IsRent | int | 是 | 租借状态(0闲置 10租用) |
| SellerName | string | 否 |当前租用企业名称 |
| IsPublic | int | 是 | 是否公共资源 |
| CalculateType| int | 是 |计价方式（1面积 2一口价） |







> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList |array int | 否 | 数据范围树枝叶编码列表 |
| KeyWord | string | 否 | 关键字|
| ParkFloorSysNo | int | 是 | 楼层系统编码 |
| IsRentList | array int | 是 | 租借状态 (0闲置 10租用) |
|IsPublicList|array int | 是 |是否公共资源 |
| BuildingSysNo | int | 是 | 楼宇系统编码 |
| ParkSysNo | int | 是 | 园区编码 |
|ParkRoomTypeList  |array  int | 是 |房间类型|
|StartBuildingArea|decimal | 是 |开始面积 |
|EndBuildingArea|decimal | 是 |截至面积 |










> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





