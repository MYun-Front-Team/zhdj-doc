# 获取监视设备详情

##### _【功能说明】_ {#【功能说明】}

获取监视设备详情

_**【应用场景】**_

获取监视设备详情

_**【接口地址】**_

http://ip:port/UMQuery/DeviceStatus/GetDeviceStatusBySysNo
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |
| DeviceTime| datetime| 是 | 当前设备时间|



> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校…… |
| DataRangeSysNo| int| 是 | 学校数据范围编码 |
| DeviceName| string| 是 | 设备名称 |
| DeviceCode| string| 是 | 设备唯一编码 |
| HeartBeat| string| 是 | 最后心跳时间|
| HeartStatus| int | 是 |状态（0初始，10正常，9警告，11下线） |
| JsonObj| string| 是 | 备注 |
| GroupInfos|array[GroupInfo] | 是 | 所有相关分组信息|
| ReceiveMessageCount| int| 否 | 接收消息次数 |



> #### GroupInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TemplateSysNo| int | 是 | 当前模板编码|
| TemplateCode| string| 是 | 当前模板编码|
| TemplateName| string| 是 | 当前模板名称|
| GroupName| string| 是 | 当前分组名称|
| GroupSysNo| int | 是 | 当前分组编码|
| SortNo| int | 是 | 排序|
| StartDate| datetime| 是 | 开始展示时间|
| EndDate| datetime| 是 | 结束展示时间|





