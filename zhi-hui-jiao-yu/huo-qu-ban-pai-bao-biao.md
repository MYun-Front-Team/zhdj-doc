# 获取班排报表

##### _【功能说明】_ {#【功能说明】}

获取班排报表


_**【应用场景】**_

获取班排报表


_**【接口地址】**_

http://ip:port/EduQuery/Report/GetDeviceReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceTemplates | array[DeviceTemplate] | 是 | 模板统计|
| DeviceGroups | array[DeviceGroup] | 是 | 分组统计|
| HeartStatusGroups | array[HeartStatusGroup] | 是 | 状态统计|






> #### DeviceTemplate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TemplateCode| int | 是 | 模板编号 |
| TemplateName| int | 是 | 模板名称 |
| Count| int | 是 | 设备数量 |

> #### DeviceGroup

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupName| int | 是 | 分组名称 |
| Count| int | 是 | 设备数量 |

> #### HeartStatusGroup

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HeartStatus|int | 是 |状态（0初始，10正常，9警告，11下线） |
| Count| int | 是 | 设备数量 |













