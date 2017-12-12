# 新增收藏 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增收藏

_**【应用场景】**_

新增收藏

注：1、Module的4要素表示收藏的对象，如商品、店铺等等；

2、根据UserSysNo找到收藏人Person；

3、判断重复收藏；

_**【接口地址】**_

[http://ip:port/DealAction/](http://ip:port/HMAction/River/AddRiver)Favorite[/A](http://ip:port/HMAction/River/AddRiver)ddFavorite

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 否 | 买家组织系统编码 |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FavoriteSysNo | int | 是 | 系统编码 |



