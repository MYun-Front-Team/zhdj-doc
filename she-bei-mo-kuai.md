# 设备模块-字段说明 {#新增河流}

> #### Equipment基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备系统编码 |
| OrganizationSysNo | int | 是 | 产权所属组织系统编码 |
| OrganizationName | string | 是 | 产权所属组织 |
| DataRangeSysNo | int | 是 | 数据范围编码列表 |
| DataRangeName | string | 是 | 数据范围名称 |
| PersonSysNo | int | 是 | 产权人编码 |
| PersonName | string | 是 | 产权人姓名 |
| CellPhoneNo | string | 是 | 产权人手机 |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| Passageway | int | 是 | 货道数量 |
| SN | string | 是 | SN号 |
| EquipmentName | string | 是 | 设备名称 |
| PCDCode | string | 是 | PCD代码 |
| PCDDescription | string | 是 | PCD描述 |
| Location | string | 是 | 具体位置 |
| QCCode | string | 是 | 二维码 |
| EquipmentStatus | int | 是 | 设备状态10正常 11故障 |
| OnlineStatus | int | 是 | 在线状态10在线 11离线 |
| FaultType | string | 否 | 故障类型描述 |
| FaultTime | datetime | 否 | 故障时间 |
| LineSysNo | int | 否 | 线路编码 |
| LineName | string | 否 | 线路名称 |
| PassagewayList | array object | 否 | 货道商品列表 |
|  |  |  |  |

**Passageway货道商品**

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备编码 |
| PassagewayNo | int | 是 | 货道号 |
| ProductGroupSysNo | int | 是 | 商品编码 |
| ProductGroupName | string | 是 | 商品名称 |
| ImgList | array string | 是 | 图片列表 |
| SalePrice | decimal\(18,2\) | 是 | 销售价格 |
| OutStock | int | 是 | 10正常，11缺货 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 产权人所属组织系统编码 |
| PersonSysNo | int | 否 | 产权人编码 |
| Keywords | string | 否 | 关键字搜索 |
| EquipmentTypeSysNoList | array int | 否 | 设备类型编码列表 |
| EquipmentStatusList | array int | 否 | 设备状态列表 |
| OnlineStatusLIst | array int | 否 | 在线状态列表 |
| LineSysNoList | array int | 否 | 线路编码列表 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPassageway | int | 否 | 是否显示货道商品 |



