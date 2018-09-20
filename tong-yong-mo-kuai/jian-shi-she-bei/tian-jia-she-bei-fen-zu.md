# 添加设备分组

##### _【功能说明】_ {#【功能说明】}

添加设备分组

_**【应用场景】**_

添加设备分组

_**【接口地址】**_

http://ip:port/UMAction/DeviceStatus/AddDeviceGroup


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo| int| 是 | 学校数据范围编码 |
| TemplateSysNo| int| 是 | 模板编码|
| GroupName| string| 是 | 分组名称|
| Remark| string| 否 | 备注|
| JsonObj| string| 否 | 自定义对象|
| SortNo| int| 否 | 排序|
| StartDate| datetime| 是 | 开始时间|
| EndDate| datetime| 是 | 结束时间|



> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 是 | 系统编码 |



