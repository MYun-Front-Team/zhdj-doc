# 获取购物车数量 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取购物车数量

_**【应用场景】**_

获取购物车数量

_**【接口地址】**_

[http://ip:port/DealQuery/](http://ip:port/HMAction/River/AddRiver)Deal[/G](http://ip:port/HMAction/River/AddRiver)etCartCount

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CartCount | int | 是 | 购物车数量 |



