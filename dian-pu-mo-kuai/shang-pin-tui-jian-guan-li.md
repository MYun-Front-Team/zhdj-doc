# 商品推荐管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 推荐组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（店铺树） |
| RecommendSysNo | int | 是 | 推荐系统编码 |
| RecommendType | int | 是 | 类型：0首页推荐，1特惠…… |
| CategorySysNo | int | 否 | 推荐行业系统编码 |
| AreaSysNo | int | 否 | 推荐区域系统编码 |
| PCDCode | string | 否 | 推荐区域PCDCode |
| PCDDesc | string | 否 | 推荐区域PCD描述 |
| RecommendStartTime | string | 是 | 启用开始时间 |
| RecommendEndTime | string | 是 | 启用结束时间 |
| Remark | string | 否 | 备注 |
| Organization | object | 否 | 组织 |
| Seller | object | 否 | 商家 |
| Shop | object | 否 | 店铺 |
| Product | object | 否 | 商品（简版） |
| Distance| decimal| 否 | 距离|
| RecommendObjType| int | 否 | 推荐对象类型0(商品) 1店铺 |


> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendStatus | int | 否 | 推荐状态：0未开始，1进行中，2已过期 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |

### Product

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |
| PriceRuleType| int | 是 | 定价规则（0款，1SKU） |
| ProductGroupName| STRING | 是 | 规格名称|
| ProductGroupClassSysNo| int| 是 | 类别编码|
| ProductGroupClassName| STRING | 是 | 类别名称|
| ProductGroupMemo| STRING | 是 | 款备注|
| FileThumbnailUrlList|array STRING | 是 |缩略图|
| Price| Price| 是 | 价格|
| UnitList| array[Unit]| 是 | 单位|
| OrganizationSysNo| int| 是 | 组织号|
| DataRangeSysNo| int | 是 | 店铺数据范围|
| DataRangeName| STRING | 是 | 店铺数据范围|
| SkuList| array[Sku]| 是 | sku|
| TagList| array[Tag]| 是 |标签|

### Sku

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo| int | 是 | 系统编码 |
| SkuName|STRING | 是 | sku名称|
| BarCode| STRING | 是 | 条码 |
| Price| Price| 是 | 价格|
| FileThumbnailUrlList|array[ STRING] | 是 | sku缩略图|



> #### Price说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CostPrice | decimal\(18,2\) | 否 | 成本价 |
| MarketPrice | decimal\(18,2\) | 否 | 市场价 |
| SalePrice | decimal\(18,2\) | 否 | 销售价 |
| MaxSalePrice | decimal\(18,2\) | 否 | 最大销售价 |
| PointPrice | decimal\(18,2\) | 否 | 积分价格 |
| MinCutSalePrice | decimal\(18,2\) | 否 | 最低砍价 |



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围系统编码（投放位置树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| RecommendStatusList | array int | 否 | 推荐状态：0未开始，1进行中，2已过期 |
| RecommendTypeList | array int | 否 | 推荐类型 |
| AreaSysNo | int | 否 | 推荐区域系统编码 |
| CategorySysNo | int | 否 | 推荐行业系统编码 |
| PCDDesc | string | 否 | 推荐区域PCD描述 |
| Longitude| deciaml | 否 | Longitude|
| Latitude| deciaml | 否 | Latitude|

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowSeller | int | 否 | 是否显示商家 |
| IsShowShop | int | 否 | 是否显示店铺 |
| IsShowHollowTime | int | 否 | 是否启用坑位时间（一旦启用，那么当前时间必须在启用时间范围内，适用前台） |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



