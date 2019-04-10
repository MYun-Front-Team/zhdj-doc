# 处理预警

_**【接口地址】**_

http://ip:port/VDAction/Detect/HandleAlarm

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmSysNoList | array[int] | 是 | 预警id列表 |
| HandleProc | string | 否 | 处理过程 |
| HandleResult | int | 是 | 1整改， 2处罚， 3其他|

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


