# 获取燃油消耗量及安全核查列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetFuelSafetyList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 检测站组织编码 |
| vehicleType | string | 否 | 挂车，牵引车，客车，货车，专项作业车，其他 |
| StartRegistDate | datetime | 否 | 注册日期起 |
| EndRegistDate | datetime | 否 | 注册日期止 |
| vehicleNo | string | 否 | 车牌号码 |

> #### _应答数据 _（数组） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FuelSafetySysNo | int | 是 | 燃油消耗量及安全核查id |
| OrganizationSysNo | int | 是 | 检测站组织名称 |
| dsName | string | 是 | 检测机构名称 |
| vehicleType | string | 是 | 挂车，牵引车，客车，货车，专项作业车，其他 |
| vehicleTypeName | string | 是 | 车辆类型 |
| registDate | datetime | 是 | 注册日期 |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| vehicleBrandModel | string | 是 | 品牌型号 |
| safetyResult | string | 是 | 安全核查结果 |
| fuelResult | string | 是 | 燃油消耗量核查结果 |
| CreateTime | datetime | 是 | 创建时间 |
| LastModifyTime | datetime | 是 | 更新时间 |



