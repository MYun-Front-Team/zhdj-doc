# 获取大数据 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetHugeDataReport](http://ip:port/WTQuery/Water/GetNationReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据_ {#应答数据-（巡河记录数组）}

#### HugeDataReport {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CityNum | int | 是 | 市级数量 |
| HouseEstateNum | int | 是 | 小区数量 |
| WaterTankNum | int | 是 | 水箱数量 |
| TodayNormalWaterTankNum | int | 是 | 今日正常水箱数 |
| TodayAlarmWaterTankNum | int | 是 | 今日问题水箱数 |
| WeekAlarmWaterTankList | array WeekAlarmWaterTank | 是 | 本周问题水箱数列表 |
| WeekAlarmRateList | array WeekAlarmRate | 是 | 本周问题占比列表 |
| CityList | array CityData | 是 | 城市列表 |

WeekAlarmWaterTank

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Date | datetime | 是 | 日期 |
| Number | int | 是 | 数量 |

WeekAlarmRate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Name | string | 是 | 名称 |
| Rate | decimal | 是 | 比例 |

CityData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| WaterTankNum | int | 是 | 水箱数 |



