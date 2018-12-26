# 获取市级地图 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetCityReport](http://ip:port/WTQuery/Water/GetNationReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PCDCode | string | 是 | 省市区编码 |

> #### _应答数据_ {#应答数据-（巡河记录数组）}

#### CityReport {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateNum | int | 是 | 小区总数 |
| AlarmHouseEstateNum | int | 是 | 预警小区数 |
| NormalHouseEstateNum | int | 是 | 正常小区数 |
| FaultHouseEstateNum | int | 是 | 故障小区数 |
| HouseEstateList | array HouseEstateData | 是 | 小区列表 |

HouseEstateData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |
| HouseEstateName | string | 是 | 小区名称 |
| ContactPerson | string | 是 | 负责人 |
| ContactPhone | string | 是 | 联系电话 |
| Longitude | deciaml | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| WaterTankNum | int | 是 | 水箱数 |
| WaterTankStatus | int | 是 | 1正常，11预警 |



