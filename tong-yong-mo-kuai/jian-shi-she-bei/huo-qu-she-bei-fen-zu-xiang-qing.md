# 获取设备分组详情

##### _【功能说明】_ {#【功能说明】}

获取设备分组详情


_**【应用场景】**_

获取设备分组详情


_**【接口地址】**_

http://ip:port/UMQuery/DeviceStatus/GetDeviceGroupBySysNo
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceGroupSysNo | int | 是 | 分组系统编码 |




> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceGroupSysNo | int | 是 | 分组系统编码 |
| DataRangeSysNo| int| 是 | 学校数据范围编码 |
| TemplateSysNo| int| 是 | 模板编码|
| TemplateCode| string| 是 | 模板编码|
| TemplateName| string| 是 | 模板名称|
| GroupName| string| 是 | 分组名称|
| Remark| string| 是 | 备注|
| JsonObj| string| 是 | 自定义对象|
| SortNo| int| 是 | 排序|
| StartDate| datetime| 是 | 开始时间|
| EndDate| datetime| 是 | 结束时间|
| DeviceCount| int| 是 | 设备数量|

