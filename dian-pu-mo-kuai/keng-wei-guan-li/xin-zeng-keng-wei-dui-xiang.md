# 新增坑位对象

##### _【功能说明】_ {#【功能说明】}
新增坑位对象

_**【应用场景】**_
新增坑位对象

_**【接口地址】**_

http://ip:port/ShopAction/Hollow/AddHollowObject

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |
| HollowObjectList| array[HollowObject ] | 是 | 对象列表 |


> #### HollowObject {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| OrganizationSysNo | int | 是 | 商品组织系统编码 |




