# 新增价格方案 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增价格方案

_**【应用场景】**_

新增价格方案

注：如是商品类价格：ModuleSourceClass=0代表款，ModuleSourceClass=1代表SKU

_**【接口地址】**_

[http://ip:port/UMAction/PriceGroup/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etPriceGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围结点列表（店铺树） |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| PriceGroupList | array object | 是 | 价格组列表 |

> #### PriceGroup {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PriceGroupName | string | 否 | 价格组名称代码（与类型匹配枚举） |
| PriceGroupType | int | 是 | 价格组类型：1阶梯价，2客户等级折扣价，3客户等级阶梯价，4客户阶梯价 |
| ~~ShopLevelSysNo~~ | ~~int~~ | ~~否~~ | ~~店铺等级系统编码~~ |
| CustomerLevelSysNo | int | 否 | 客户等级系统编码 |
| CustomerSysNo | int | 否 | 客户系统编码 |
| QuantityRange | object | 否 | 商品数量范围系统编码 |
| Rate | decimal\(18,2\) | 否 | 折扣 |
| IsEnable | int | 是 | 是否启用 |
| PriceType | int | 是 | 价格类型：1成本价，2市场价，3销售价，4积分价格 ，5砍价最低价,6佣金|
| PriceCode | string | 否 | 价格代码（与类型匹配枚举） |
| Price | decimal\(18,2\) | 否 | 价格 |

#### QuantityRange {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaxQuantity | int | 是 | 购买数量上限 |
| MinQuantity | int | 是 | 购买数量下限 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



