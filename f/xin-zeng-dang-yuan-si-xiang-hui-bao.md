# 新增汇报 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增汇报

_**【应用场景】**_

新增汇报

_**【接口地址】**_

[http://ip:port/UMAction/Report/Add](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)Report

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| ReportTime | string | 是 | 汇报时间 |
| ReportTitle | string | 是 | 汇报抬头 |
| ReportContent | string | 是 | 汇报说明 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 文件图片Path列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 系统编码 |



