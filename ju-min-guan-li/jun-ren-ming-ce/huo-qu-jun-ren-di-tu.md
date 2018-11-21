# 获取军人地图

##### _【功能说明】_ {#【功能说明】}

获取民兵地图

_**【应用场景】**_

获取民兵地图

_**【接口地址】**_

[http://ip:port/ResidentQuery/Resident/GetResidentSoldierYearMap](http://ip:port/ResidentQuery/Resident/GetResidentSoldierMap)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 否 | 数据范围树编码列表 |
| SoldierType | int | 否 | 民兵类型（1干部2党支部） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName | int | 是 | 数据范围树名称 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| Items | array\[Item\] | 是 | 军人信息 |

#### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Lat | decimal | 是 | 纬度 |
| Lon | decimal | 是 | 经度 |
| Name | string | 是 | 军人姓名 |



