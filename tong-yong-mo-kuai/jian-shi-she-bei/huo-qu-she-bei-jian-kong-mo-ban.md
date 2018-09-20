# 获取设备模板列表

##### _【功能说明】_ {#【功能说明】}

获取设备模板列表


_**【应用场景】**_

获取设备模板列表


_**【接口地址】**_

http://ip:port/UMQuery/DeviceStatus/GetDeviceTemplateList
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo| int| 是 | 学校数据范围编码 |





> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceTemplateSysNo | int | 是 | 系统编码 |
| DataRangeSysNo| int| 是 | 学校数据范围编码 |
| TemplateCode| string| 是 | 模板编码|
| TemplateName| string| 是 | 模板名称|
| Remark| string| 是 | 备注|
| JsonObj| string| 是 | 自定义对象|


