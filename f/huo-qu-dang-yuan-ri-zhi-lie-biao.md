# 获取日志列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取日志列表

_**【应用场景】**_

获取日志列表

_**【接口地址】**_

[http://ip:port/UMQuery/ActionLog/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)LogList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceSysNo | int | 是 | 模块来源系统编码 |
| ActionType | int | 否 | 日志类型（枚举） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LogSysNo | int | 是 | 日志系统编码 |
| ActionType | int | 是 | 日志类型（枚举） |
| ActionTime | string | 是 | 日志时间 |
| ActionName | string | 是 | 日志说明 |
| ActionDescription | string | 否 | 日志描述 |



