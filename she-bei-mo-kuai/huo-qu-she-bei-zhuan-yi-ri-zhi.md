# 获取设备转移日志 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetTransformLogList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNoList | array\[int\] | 否 | 设备编码 |

> #### _应答数据 （数组）TransformLog_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备编码 |
| SN | string | 是 | SN码 |
| PersonFromSysNo | int | 是 | 转出人编码 |
| PersonFromName | string | 是 | 转出人姓名 |
| PersonFromCellPhoneNo | string | 是 | 转出人手机 |
| PersonToSysNo | int | 是 | 转入人编码 |
| PersonToName | string | 是 | 转入人姓名 |
| PersonToCellPhoneNo | string | 是 | 转入人手机 |
| TransformTime | datetime | 是 | 转移时间 |
| Remark | string | 否 | 备注 |



