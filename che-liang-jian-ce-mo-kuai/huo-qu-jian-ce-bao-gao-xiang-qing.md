# 获取检测报告详情 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetDetectRecordBySysNo](http://ip:port/VDQuery/Detect/GetDetectRecordBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| detectRecordSysNo | int | 是 | 检验报告id |

> #### _应答数据 \_DetectRecord_（数组） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| detectRecordSysNo | int | 是 | 检测报告id |
| detectSn | string | 是 | 检测流水号 |
| dsId | string | 是 | 检测机构唯一编码 |
| dsName | string | 是 | 检测机构名称 |
| detectDate | string | 是 | 检测日期 |
| detectType | string | 是 | 检测类别 |
| jcyxqz | string | 是 | 车辆检测有效期止\(月末\) |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| vinNo | string | 是 | 车辆识别号码 |
| engineNo | string | 是 | 发动机号码 |
| travelMileage | decimal | 是 | 行程总里程 |
| fuelType | string | 是 | 燃油类别 |
| farLightCanAdjust | string | 是 | 远光束能否单独调整 |
| steeringAxleAmount | decimal | 是 | 转向轴数 |
| detectTotalCount | decimal | 是 | 总检次数 |
| vehicleType | string | 是 | 车辆类型 |
| registDate | string | 是 | 注册日期 |
| busTypeLevel | string | 是 | 客车类型与等级 |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
| detectResult | string | 是 | 检验结果 |
| detectSafeyResult | string | 是 | 安全检测结果 |
| uploadStatus | int | 是 | 上传状态 1待上传，10已上传，11不上传 |
| uploadTime | datetime | 是 | 上传时间 |
| requireStatus | int | 是 | 10正常，11市平台要求字段未填写 |
| tempStatus | int | 是 | 10正常，11临时牌照未修改 |
| abnormalStatus | int | 是 | 10正常，11在异常名单内 |



