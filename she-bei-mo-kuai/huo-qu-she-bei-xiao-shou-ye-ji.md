# 获取设备销售业绩 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetEqmSaleReport](http://ip:port/EqmQuery/Equipment/GetSaleReport)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LineSysNoList | array\[int\] | 否 | 路线数组 |

> #### _应答数据 \(数组\)_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备系统编码 |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| SN | string | 是 | SN号 |
| PCDCode | string | 是 | PCD代码 |
| PCDDescription | string | 是 | PCD描述 |
| Location | string | 是 | 具体位置 |
| LineSysNo | int | 是 | 线路编码 |
| LineName | string | 是 | 线路名称 |
| Amount | decimal | 是 | 金额 |
| Online | decimal | 是 | 移动金额 |
| Cash | decimal | 是 | 现金 |
|  |  |  |  |



