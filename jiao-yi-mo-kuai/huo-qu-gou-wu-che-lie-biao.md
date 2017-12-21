# 获取购物车列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取购物车列表

_**【应用场景】**_

获取购物车列表

_**【接口地址】**_

[http://ip:port/DealQuery/](http://ip:port/HMAction/River/AddRiver)Deal[/G](http://ip:port/HMAction/River/AddRiver)etCartList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| CustomizedSpecValue | string | 否 | 可定制规格值 |
| ~~Quantity~~ | ~~int~~ | ~~是~~ | ~~数量~~ |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 卖家组织系统编码 |
| OrganizationName | string | 是 | 卖家组织名称 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| DataRangeName | string | 是 | 数据范围结点名称 |
| CartList | array object | 是 | 购物车列表 |

#### Cart说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CartSysNo | int | 是 | 卖家组织系统编码 |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| ~~ModuleSourceName~~ | ~~string~~ | ~~是~~ | ~~来源名称（如商品名称）~~ |
| CustomizedSpecValue | string | 否 | 可定制规格值 |
| Quantity | int | 是 | 数量 |
| ~~Price~~ | ~~object~~ | ~~是~~ | ~~价格实体（见商品）~~ |
| sku | object | 否 | sku实体 |



