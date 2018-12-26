# 获取小区地图 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetHouseEstateReport](http://ip:port/WTQuery/Water/GetNationReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |

> #### _应答数据_ {#应答数据-（巡河记录数组）}

#### HouseEstateReport {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |
| HouseEstateName | string | 是 | 小区名称 |
| PDCCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |
| ContactPerson | string | 是 | 负责人 |
| ContactPhone | string | 是 | 联系电话 |
| WaterTankNum | int | 是 | 水箱总数 |
| AlarmWaterTankNum | int | 是 | 预警水箱数 |
| NormalWaterTankNum | int | 是 | 正常水箱数 |
| FaultWaterTankNum | int | 是 | 故障水箱数 |
| WaterTankList | array WaterTankData | 是 | 水箱列表 |

WaterTankData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WaterTankSysNo | int | 是 | 水箱id |
| WaterTankCode | string | 是 | 水箱编号 |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |
| WaterTankStatus | int | 是 | 1正常，11预警 |



