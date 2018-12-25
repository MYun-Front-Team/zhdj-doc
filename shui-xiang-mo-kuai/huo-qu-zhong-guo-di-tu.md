# 获取中国地图 {#获取河长巡河记录}

_**【接口地址】**_

http://ip:port/WTQuery/Water/GetNationReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据_ {#应答数据-（巡河记录数组）}

#### NationReport {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CityNum | int | 是 | 市总数 |
| HouseEstateNum | int | 是 | 小区总数 |
| CityList | array CityData | 是 | 市列表 |



CityData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| HouseEstateNum | int | 是 | 小区数 |
| WaterTankNum | int | 是 | 水箱数 |
| WaterTankStatus | int | 是 | 1正常，11预警 |





