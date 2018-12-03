# 获取搜索记录列表

##### _【功能说明】_ {#【功能说明】}

获取搜索记录列表

_**【应用场景】**_

获取搜索记录列表

_**【接口地址】**_

http://ip:port/UMQuery/KeyWord/GetKeyWordList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo| int | 否 | 模块系统编码 |
| ModuleSourceType| int | 否 | 模块来源类型 |
| ModuleSourceSysNo| int | 否 | 模块来源编码 |
| ModuleSourceClass| int | 否 | 模块来源类别 |

> #### KeyWord {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWordSysNo| int | 否 | 系统编码 |
| SearchKey| string | 是 |关键字|






