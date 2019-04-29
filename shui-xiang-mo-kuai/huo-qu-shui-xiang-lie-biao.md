# 获取水箱列表

_**【接口地址】**_

http://ip:port/WTQuery/Water/GetWaterTankList

> #### _请求数据_ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 登录人id |
| HouseEstateSysNo | int | 否 | 小区id |
| PCDDescription | string | 否 | 省市区名称 |
| HouseEstateName | string | 否 | 小区名称 |
| WaterTankCode | string | 否 | 水箱编号 |

> #### _应答数据 _（数组） 

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
| CapAlarm | int | 是 | 0水箱盖开启报警，1不报警 |
| WaterTankStatus | int | 是 | 1正常，11预警 |
| SyncTime | datetime | 是 | 最后同步时间 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| ClearType | int | 是 | 清洗类型：0自动，1手动 |
| LidStatus | int | 是 | 水箱盖状态：0锁定，1开启 |
| Door2 | int | 是 | 进水常开电磁阀0常开，1常闭 |
| Door3 | int | 是 | 排污常闭电磁阀0常闭，1常开 |
| Door4 | int | 是 | 上端清洗水常闭电磁阀0常闭，1常开 |
| Door5 | int | 是 | 下端清洗水常闭电磁阀0常闭，1常开 |
| StaState | int | 是 | 站点状态0：断开；1：正常；2：故障 |
| ComState | int | 是 | 通信状态1：正常；2：故障 |
| AlarmRuleList | array AlarmRule | 是 | 预警规则数组 |
| OtherParamList | array OtherParam | 是 | 其它参数数组 |

AlarmRule

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmRuleSysNo | int | 是 | 预警规则id |
| WaterTankSysNo | int | 是 | 水箱id |
| AlarmName | string | 是 | 规则名称 |
| UpperLimit | decimal | 是 | 上限 |
| LowerLimit | decimal | 是 | 下限 |
| Unit | string | 是 | 单位 |
| CurrentValue | string | 是 | 当前读数，""代表尚未读取 |
| RuleStatus | int | 是 | 0 尚未读取数据，1正常，10报警 |

OtherParam

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OtherParamSysNo | int | 是 | 参数id |
| WaterTankSysNo | int | 是 | 水箱id |
| ParamName | string | 是 | 参数名称 |
| Unit | string | 是 | 单位 |
| CurrentValue | string | 是 | 当前读数，""代表尚未设置 |





