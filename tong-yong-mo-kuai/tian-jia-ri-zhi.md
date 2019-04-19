# 添加日志

##### _【功能说明】_ {#【功能说明】}

添加日志

_**【应用场景】**_

添加日志

_**【接口地址】**_
http://ip:port/UMAction/ActionLog/AddLog

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceSysNo | int | 是 | 模块来源系统编码 |
| ActionType | int | 否 | 日志类型（枚举） |
| ActionName|string | 否 | 日志名称 |
| ActionDescription|string | 否 | 日志描述 |
| IsShow | int | 否 | 是否显示 |




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 是 | 日志系统编码 |



