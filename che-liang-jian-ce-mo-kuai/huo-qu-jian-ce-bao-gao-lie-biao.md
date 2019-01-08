# 获取检测报告列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetDetectRecordList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsName | string | 否 | 机构名称 |
| StartDetectDate | datetime | 否 | 检测日期起 |
| EndDetectDate | datetime | 否 | 检测日期止 |
| vehicleNo | string | 否 | 车牌号码 |
| plateColorCode | string | 否 | 车牌颜色代码 |
| uploadStatusList | array\[int\] | 否 | 1待上传，10已上传，11不上传 |

> #### _应答数据 \_DetectRecord_（数组） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| detectRecordSysNo | int | 是 | 检测报告id |
| detectSn | string | 是 | 检测流水号 |
| dsName | string | 是 | 检测机构名称 |
| detectDate | string | 是 | 检测日期 |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| uploadStatus | int | 是 | 上传状态 1待上传，2暂停上传，10已上传，11不上传 |
| uploadTime | datetime | 是 | 上传时间 |
| requireStatus | int | 是 | 10正常，11市平台要求字段未填写 |
| tempStatus | int | 是 | 10正常，11临时牌照未修改 |
| abnormalStatus | int | 是 | 10正常，11在异常名单内 |
| CreateTime | datetime | 是 | 创建时间 |



