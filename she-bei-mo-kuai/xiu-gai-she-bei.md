# 修改设备 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/EditEquipment](http://ip:port/EqmQuery/Equipment/GetEquipmentBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备编码 |
| SN | string | 是 | SN号 |
| EquipmentName | string | 否 | 设备名称 |
| PCDCode | string | 否 | PCD代码 |
| PCDDescription | string | 否 | PCD描述 |
| Location | string | 否 | 具体位置 |
| LineSysNo | int | 否 | 线路编码 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




