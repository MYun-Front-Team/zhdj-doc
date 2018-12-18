# 新增对象到坑位

##### _【功能说明】_ {#【功能说明】}

新增对象到坑位

_**【应用场景】**_

新增对象到坑位


_**【接口地址】**_

http://ip:port/ShopAction/Hollow/AddHollowObject

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |
|HollowObjects | array[HollowObject] | 是 |对象列表|

> #### HollowObject {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| ModuleSourceName| string | 否 | 来源系统名称 |
| HollowUrl | string | 否 | 链接地址 |
| OrganizationSysNo | int | 是 | 商品组织系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



