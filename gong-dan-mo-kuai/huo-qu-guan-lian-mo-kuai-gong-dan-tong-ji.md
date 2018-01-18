# 获取关联模块工单统计 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取关联模块工单统计

_**【应用场景】**_

获取关联模块工单统计

_**【接口地址】**_

[http://ip:port/WorkQuery/Work/GetModuleWorkStatistics](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceSysNo | int | 是 | 模块系统编码 |
| WorkStatusList | array int | 否 | 工单状态 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkType | int | 是 | 工单类型（枚举） |
| WorkCount | int | 是 | 数量 |



