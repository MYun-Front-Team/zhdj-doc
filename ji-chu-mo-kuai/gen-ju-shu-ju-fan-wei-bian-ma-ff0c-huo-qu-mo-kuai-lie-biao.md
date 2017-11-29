# 根据数据范围编码，获取模块列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据数据范围编码，获取模块列表

_**【应用场景】**_

根据数据范围编码，获取模块列表

注：如果数据范围编码没有配置，则在树上往上找已配置的模块；

_**【接口地址】**_

[http://ip:port/BasicQuery/Basic/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ModuleListByDataRangeSysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围系统编码 |
| LoginSource | int | 否 | 登录来源（枚举） |
| IsShowSystemConfig | int | 否 | 是否显示系统配置 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleList | array object | 是 | 模块列表 |
| SystemConfig | object | 是 | 系统配置 |

> #### Module说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块系统编码 |
| ModuleName | string | 是 | 模块名称 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceName | string | 否 | 来源名称 |
| SortNo | int | 是 | 排序 |

#### SystemConfig说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EntranceUrl | string | 是 | 首页Top入口图 |



