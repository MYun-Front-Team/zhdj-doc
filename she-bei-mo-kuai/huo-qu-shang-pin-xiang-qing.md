# 获取商品详情 {#获取河长巡河记录}

_**【接口地址】**_

http://ip:port/EqmQuery/Equipment/GetEqmProductBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 商品编码 |

> #### _应答数据 EqmProduct_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 商品编码 |
| ProductGroupName | string | 是 | 商品名称 |
| ImgList | array string | 是 | 图片列表 |
| SalePrice | decimal\(18,2\) | 是 | 销售价格 |
| EquipmentTypeList | array object | 是 | 适用设备类型列表 |

#### _EquipmentType_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| EquipmentNum | int | 是 | 设备数量 |
| Passageway | int | 是 | 货道数量 |



