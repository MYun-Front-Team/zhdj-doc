# 新增购物车 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增购物车

_**【应用场景】**_

新增购物车

注：判断是否存在同样的存放记录，不存在则新增，存在则累计；

_**【接口地址】**_

[http://ip:port/DealAction/](http://ip:port/HMAction/River/AddRiver)Deal[/A](http://ip:port/HMAction/River/AddRiver)ddCart

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| CustomizedSpecValue | string | 否 | 可定制规格值 |
| Quantity | int | 是 | 数量 |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| Remark | string | 否 | 备注|


> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CartSysNo | int | 是 | 购物车系统编码 |



