# 新增搜索记录

##### _【功能说明】_ {#【功能说明】}

新增搜索记录

_**【应用场景】**_

新增搜索记录

_**【接口地址】**_

http://ip:port/UMAction/KeyWord/AddKeyWord

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo| int | 否 | 模块系统编码 |
| ModuleSourceType| int | 否 | 模块来源类型 |
| ModuleSourceSysNo| int | 否 | 模块来源编码 |
| ModuleSourceClass| int | 否 | 模块来源类别 |
| SearchKey| string | 是 |关键字|


> #### KeyWord {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWordSysNo| int | 否 | 系统编码 |






