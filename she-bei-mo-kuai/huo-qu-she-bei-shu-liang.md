# 获取设备数量 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetEquipmentNum](http://ip:port/EqmQuery/Equipment/GetEquipmentNum)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total | int | 是 | 总数 |
| Online | int | 是 | 在线 |
| Offline | int | 是 | 离线 |
| News | int | 是 | 新增 |



