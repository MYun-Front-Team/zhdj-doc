# 获取汇报列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取汇报列表

_**【应用场景】**_

获取汇报列表

_**【接口地址】**_

[http://ip:port/UMQuery/Report/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| ReportStartTime | string | 否 | 汇报开始时间 |
| ReportEndTime | string | 否 | 汇报结束时间 |
| KeyWord | string | 否 | 关键字（标题） |
| IsOwner | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 系统编码 |
| ReportTime | string | 是 | 时间 |
| ReportTitle | string | 是 | 主题 |
| ReportContent | string | 是 | 内容 |
| Remark | string | 否 | 备注 |
| ReportPerson | object | 否 | 人员实体对象（简版） |



