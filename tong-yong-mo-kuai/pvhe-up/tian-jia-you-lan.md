#添加游览

##### _【功能说明】_ {#【功能说明】}

添加游览

_**【应用场景】**_



_**【接口地址】**_

http://ip:port/UMAction/PVAndUV/AddPVAndUV


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 是 | 人员编码编码 |
| ModuleRelations| array[ModuleRelation]| 否 | 附属模块|



#### ModuleRelation

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceType | int | 否 | 关联模块类型 |
| ModuleSourceClass | int | 否 | 关联模块分类 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |








> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




