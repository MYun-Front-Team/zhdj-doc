# 新增水箱 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTAction/Water/AddWaterTank](http://ip:port/WTQuery/Water/GetWaterTankBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |
| WaterTankCode | string | 是 | 水箱编号 |
| IP | string | 是 | ip地址 |
| Location | string | 是 | 具体地址 |
| Length | decimal | 是 | 长 |
| Width | decimal | 是 | 宽 |
| Height | decimal | 是 | 高 |
| CapAlarm | int | 是 | 1水箱盖开启报警，0不报警 |
| AlarmRuleList | array AlarmRuleEdit | 是 | 预警规则数组 |

AlarmRuleEdit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmName | string | 是 | 预警名称 |
| AlarmType | string | 是 | 预警类型 |
| UpperLimit | decimal | 是 | 上限 |
| LowerLimit | decimal | 是 | 下限 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 水箱id |



