# 设置货道商品 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/SetProductPassageway](http://ip:port/EqmAction/Equipment/SetProductPassageway)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNos | array\[int\] | 是 | 设备编码列表 |
| SetPassagewayList | array object | 否 | 设置货道列表 |

SetPassageway

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 商品编码 |
| PassagewayNo | int | 是 | 货道号 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




