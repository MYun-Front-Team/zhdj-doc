# 新增水箱

_**【接口地址】**_

http://ip:port/WTAction/Water/AddWaterTank

> #### _请求数据_ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |
| WaterTankCode | string | 是 | 水箱编号 |
| IP | string | 否 | ip地址 |
| Location | string | 是 | 具体地址 |
| Length | decimal | 是 | 长 |
| Width | decimal | 是 | 宽 |
| Height | decimal | 是 | 高 |
| CapAlarm | int | 是 | 1水箱盖开启报警，0不报警 |

> #### _应答数据 _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 水箱id |



