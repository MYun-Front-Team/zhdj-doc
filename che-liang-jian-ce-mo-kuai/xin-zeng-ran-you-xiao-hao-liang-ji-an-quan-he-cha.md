# 新增燃油消耗量及安全核查 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDAction/Detect/AddFuelSafety](http://ip:port/VDAction/Detect/AddFuelSafety)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 检测站组织名称 |
| vehicleType | string | 是 | 挂车，牵引车，客车，货车，专项作业车，其他 |
| registDate | datetime | 是 | 注册日期 |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| vehicleBrandModel | string | 是 | 品牌型号 |
| safetyResult | string | 是 | 安全核查结果 |
| fuelResult | string | 否 | 燃油消耗量核查结果 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 燃油消耗量及安全核查id |



