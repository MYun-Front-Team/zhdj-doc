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

CityData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateName | string | 是 | 小区名称 |
| ContactPerson | string | 是 | 负责人 |
| ContactPhone | string | 是 | 联系电话 |
| WaterTankNum | int | 是 | 水箱数 |
| WaterTankStatus | int | 是 | 1正常，11预警 |



