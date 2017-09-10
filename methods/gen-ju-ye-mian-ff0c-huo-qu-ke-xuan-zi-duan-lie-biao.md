# 根据页面，获取可选字段列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据页面，获取可选字段列表

_**【应用场景】**_

在模块说明中，基础字段中非必须的字段，可根据项目需求在此接口中进行自定义。

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityFieldListByPage

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| PageSysNo | int | 是 | 活动模块页（枚举） |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FieldSysNo | int | 是 | 字段系统编码 |
| FieldType | int | 是 | 字段类型：0基础，1统计，2查询，3操作 |
| FieldCode | string | 是 | 字段代码 |
| FieldName | string | 是 | 字段名称 |
| SortNo | int | 是 | 排序 |
| Remark | string | 否 | 备注 |



