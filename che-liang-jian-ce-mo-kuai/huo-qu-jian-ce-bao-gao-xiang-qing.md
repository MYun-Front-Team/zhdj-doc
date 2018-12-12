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
| tractorVehicleNo | string | 是 | 单车车牌号码 |
| tractorClient | string | 是 | 单车委托人 |
| tractorVehicleBrandModel | string | 是 | 单车品牌型号 |
| tractorVinNo | string | 是 | 单车车辆识别码 |
| tractorAdministrativeAera | string | 是 | 单车行政区域 |
| tractorEngineNo | string | 是 | 单车发动机号码 |
| trailerVehicleNo | string | 是 | 挂车车牌号码 |
| trailerClient | string | 是 | 挂车委托人 |
| trailerVehicleBrandModel | string | 是 | 挂车品牌型号 |
| trailerVinNo | string | 是 | 挂车车辆识别码 |
| trailerDriveLicense | string | 是 | 挂车车辆行驶证 |
|  |  |  |  |
| detectResult | string | 是 | 检验结果 |
| detectSafeyResult | string | 是 | 安全检测结果 |
| uploadStatus | int | 是 | 上传状态 1待上传，10已上传，11不上传 |
| uploadTime | datetime | 是 | 上传时间 |
| requireStatus | int | 是 | 10正常，11市平台要求字段未填写 |
| tempStatus | int | 是 | 10正常，11临时牌照未修改 |
| abnormalStatus | int | 是 | 10正常，11在异常名单内 |

人工检测结果

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| manualTestResultSysNo | int | 是 | 人工检测结果id |
| detectRecordSysNo | int | 是 | 检测报告id |
| detectCls | string | 是 | 检测项目 |
| evaluate | string | 是 | 判定 |
| unqualifiedItem | string | 是 | 不符合项目 |

性能检测结果

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| performanceItemSysNo | int | 是 | 性能检测结果id |
| detectRecordSysNo | int | 是 | 检测报告id |
| itemCode | string | 是 | 性能检测项目 |
| detectData | string | 是 | 性能检测数据 |
| evaluate | string | 是 | 判定 |



