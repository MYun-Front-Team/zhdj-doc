# 设备转移 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/TransforEquipment](http://ip:port/EqmQuery/Equipment/GetEquipmentBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNos | array\[int\] | 是 | 设备编码列表 |
| PersonSysNo | int | 是 | 转入人编码 |
| CellPhoneNo | string | 是 | 转入人手机 |
| Remark | string | 否 | 备注 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




