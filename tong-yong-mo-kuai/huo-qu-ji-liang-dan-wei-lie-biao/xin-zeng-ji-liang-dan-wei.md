# 新增计量单位 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增计量单位

_**【应用场景】**_

新增计量单位

_**【接口地址】**_

[http://ip:port/UMAction/Unit/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddUnit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| UnitName | string | 是 | 计量单位名称 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UnitSysNo | int | 是 | 系统编码 |



