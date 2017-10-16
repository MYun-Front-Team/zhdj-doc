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
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块类型分类编码（分类） |
| Propertys | array object | 是 | 属性列表（含属性值） |



