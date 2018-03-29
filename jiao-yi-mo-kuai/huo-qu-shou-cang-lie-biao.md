# 获取收藏列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取收藏列表

_**【应用场景】**_

获取收藏列表

注：根据Module类型来返回实体对象列表

_**【接口地址】**_

[http://ip:port/DealQuery/](http://ip:port/HMAction/River/AddRiver)Favorite[/G](http://ip:port/HMAction/River/AddRiver)etFavoriteList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 买家组织系统编码 |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo| int | 否 | 来源编码 |



> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroup | object | 是 | 款实体（简） |
| Shop | object | 是 | 店铺（简） |



