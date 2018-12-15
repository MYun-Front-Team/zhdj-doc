# 获取车辆类型燃油消耗量及安全核查合格率 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetVehicleTypeFuelSafetyPassPercent](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| vehicleType | string | 否 | 挂车，牵引车，客车，货车，专项作业车，其他 |
| StartDate | datetime | 否 | 开始日期 |
| EndDate | datetime | 否 | 结束日期 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FuelPassPercent | decimal | 是 | 燃油消耗量核查合格率 |
| FuelNoPassPercent | decimal | 是 | 燃油消耗量核查不合格率 |
| SafetyPassPercent | decimal | 是 | 安全核查合格率 |
| SafetyNoPassPercent | decimal | 是 | 安全核查不合格率 |
| TotalCount | decimal | 是 | 总数 |



