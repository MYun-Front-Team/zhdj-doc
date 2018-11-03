# 获取线路列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetLineList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 运营商人员编码 |
| Keywords | string | 否 | 关键字 |

> #### _应答数据 （数组）Line_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LineSysNo | int | 是 | 线路编码 |
| LineName | string | 是 | 线路名称 |
| PersonSysNo | int | 是 | 线路所属运营商人员编码 |
| CellPhoneNo | string | 是 | 线路所属运营商人员手机 |
| PersonName | string | 是 | 线路所属运营商人员姓名 |



