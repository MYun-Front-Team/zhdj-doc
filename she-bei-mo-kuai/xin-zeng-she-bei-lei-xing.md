# 新增设备类型 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/AddEquipmentType](http://ip:port/EqmAction/Equipment/AddEquipmentType)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| Passageway | int | 是 | 货道数量 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 设备类型编码 |



