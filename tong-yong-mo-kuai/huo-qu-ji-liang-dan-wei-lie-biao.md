# 获取计量单位列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取计量单位列表

_**【应用场景】**_

获取计量单位列表

_**【接口地址】**_

[http://ip:port/UMQuery/Unit/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)UnitList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UnitSysNo | int | 是 | 计量单位系统编码 |
| UnitName | string | 是 | 计量单位名称 |



