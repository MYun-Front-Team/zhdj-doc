# 编辑水箱 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTAction/Water/EditWaterTank](http://ip:port/WTQuery/Water/GetWaterTankBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WaterTankSysNo | int | 是 | 水箱id |
| HouseEstateSysNo | int | 是 | 小区id |
| Location | string | 是 | 具体地址 |
| Length | decimal | 是 | 长 |
| Width | decimal | 是 | 宽 |
| Height | decimal | 是 | 高 |
| CapAlarm | int | 是 | 1水箱盖开启报警，0不报警 |
| AlarmRuleList | array AlarmRuleEdit | 是 | 预警规则数组 |

AlarmRuleEdit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmRuleSysNo | int | 是 | 预警规则id |
| UpperLimit | decimal | 是 | 上限 |
| LowerLimit | decimal | 是 | 下限 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  |  |  |



