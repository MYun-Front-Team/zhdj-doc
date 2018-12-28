# 获取水箱列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetWaterTankList](http://ip:port/WTQuery/Water/GetWaterTankList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 登录人id |
| HouseEstateSysNo | int | 否 | 小区id |
| PCDDescription | string | 否 | 省市区名称 |
| HouseEstateName | string | 否 | 小区名称 |
| WaterTankCode | string | 否 | 水箱编号 |

> #### _应答数据 _（数组） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WaterTankSysNo | int | 是 | 水箱id |
| HouseEstateSysNo | int | 是 | 小区id |
| HouseEstateName | string | 是 | 小区名称 |
| WaterTankCode | string | 是 | 水箱编号 |
| IP | string | 是 | IP地址 |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |
| Length | decimal | 是 | 长 |
| Width | decimal | 是 | 宽 |
| Height | decimal | 是 | 高 |
| CapAlarm | int | 是 | 1水箱盖开启报警，0不报警 |
| WaterTankStatus | int | 是 | 1正常，11预警 |
| SyncTime | datetime | 是 | 最后同步时间 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| AlarmRuleList | array AlarmRule | 是 | 预警规则数组 |

AlarmRule

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmRuleSysNo | int | 是 | 预警规则id |
| WaterTankSysNo | int | 是 | 水箱id |
| AlarmName | string | 是 | 警报名称 |
| AlarmType | string | 是 | 报警类型\(水箱硬件提供\) |
| UpperLimit | decimal | 是 | 上限 |
| LowerLimit | decimal | 是 | 下限 |



