# 获取设备类型列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetEquipmentTypeList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keywords | string | 否 | 关键字 |

> #### _应答数据 （数组）EquipmentType_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| EquipmentNum | int | 是 | 设备数量 |
| Passageway | int | 是 | 货道数量 |



