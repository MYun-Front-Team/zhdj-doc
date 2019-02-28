# 获取预警列表

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetAlarmList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keywords | string | 否 | 关键字 |
| vehicleType | string | 否 | 车辆类型 |
| StartDetectDate | datetime | 否 | 检测日期起 |
| EndDetectDate | datetime | 否 | 检测日期止 |
| vehicleNo | string | 否 | 车牌号码 |
| HandleStatusList | array[int] | 否 | 1未处理，10已处理 |

> #### _应答数据 _（数组）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AlarmSysNo | int | 是 | 预警id |
| OrganizationSysNo | int | 是 | 检测站组织id |
| detectSn | string | 是 | 检测流水号 |
| dsId | string | 是 | 检测机构代码 |
| dsName | string | 是 | 检测机构名称 |
| vehicleType | string | 是 | 车辆类型 |
| detectDate | datetime | 是 | 检测日期 |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| vehicleBrandModel | string | 是 | 品牌型号 |
| Reason | string | 是 | 预警原因 |
| HandleStatus | int | 是 | 1未处理，10已处理 |



