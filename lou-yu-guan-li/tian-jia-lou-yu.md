# 添加楼宇

##### _【功能说明】_ {#【功能说明】}

添加楼宇

_**【应用场景】**_

添加楼宇

_**【接口地址】**_

http://ip:port/ParkAction/IndustryPark/AddBuilding

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkSysNo | int | 是 | 园区编码 |
| BuildingType | int | 是 |楼宇类型|
| BuildingClassSysNo | int | 否 | 楼宇分类（枚举） |
| BuildingName | string | 否 | 楼宇名称 |
| BuildingAddress | string | 否 | 地址 |
| BuildingPerson| string | 否 |联系人|
| BuildingPersonPhone| string | 否 |联系电话|
| Remark| string | 否 |备注|
| TotalArea| decimal | 否 |用地面积|
| BuildingArea| decimal | 否 |总建筑面积|
| BusinessArea| decimal | 否 |商务办公面积|
| ParkingLotArea| decimal | 否 |停车场面积|
| ParkingLotCount| int | 否 |机动车泊位数|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BuildingSysNo | int | 是 | 楼宇系统编码 |


