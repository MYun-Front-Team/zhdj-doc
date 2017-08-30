# 新增业务属性列表 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

新增业务属性列表

_**【应用场景】**_

新增业务属性列表

_**【接口地址】**_

[http://ip:port/UMAction/Property/AddObjectPropert](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ys

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceType | int | 是 | 来源类型 |
| SourceSysNo | int | 是 | 来源编码 |
| ObjectPropertys | array object | 是 | 属性值列表 |

> #### ObjectPropertys说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertySysNo | int | 是 | 属性系统编码 |
| PropertyValue | string | 是 | 属性值 |



