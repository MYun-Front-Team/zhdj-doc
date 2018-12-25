# 获取预警列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetAlarmList](http://ip:port/WTQuery/Water/GetWaterTankList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 登录人id |
| PCDDescription | string | 否 | 省市区名称 |
| HouseEstateName | string | 否 | 小区名称 |
| AlarmStatusList | array int | 否 | 1未处理，10已处理 |

> #### _应答数据 _（数组） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmSysNo | int | 是 | 预警id |
| HouseEstateSysNo | int | 是 | 小区id |
| WaterTankSysNo | int | 是 | 水箱id |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |
| AlarmTime | datetime | 是 | 预警时间 |
| AlarmName | string | 是 | 警报名称 |
| AlarmType | string | 是 | 报警类型\(水箱硬件提供\) |
| AlarmValue | decimal | 是 | 警报数值 |
| AlarmContent | string | 是 | 预警内容 |
| AlarmStatus | int | 是 | 1未处理，10已处理 |





