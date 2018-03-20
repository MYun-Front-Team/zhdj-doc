# 商品模块-字段说明 {#新增河流}

> #### ProductGroup基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围编码列表（店铺树） |
| DataRangeName | string | 是 | 数据范围名称 |
| ProductGroupSysNo | int | 是 | 系统编码 |
| ProductGroupType | int | 是 | 类型（枚举） |
| ProductGroupClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| ProductGroupClassName | string | 否 | 分类名称（类别树） |
| IndustryClassSysNo | int | 否 | 类型分类系统编码（行业树） |
| IndustryClassName | string | 否 | 分类名称（行业树） |
| ProductGroupCode | string | 是 | 款号 |
| ProductGroupName | string | 是 | 款名称 |
| ProductGroupDetail | string | 否 | 款描述 |
| ProductGroupMemo | string | 否 | 款备注 |
| PCDCode | string | 否 | 产地PCD代码 |
| PCDDescription | string | 否 | 产地PCD描述 |
| GoodsWeight | decimal\(18,2\) | 否 | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否 | 体积 |
| Pinyin | string | 否 | 款名称拼音 |
| FileThumbnailPathList | array string | 否 | 缩略图Path列表（第一张为首图） |
| FileMasterPathList | array string | 否 | 主图Path列表（第一张为首图） |
| FileThumbnailUrlList | array string | 否 | 缩略图Url列表（第一张为首图） |
| FileMasterUrlList | array string | 否 | 主图Url列表（第一张为首图） |
| FileDetailPathList | array string | 否 | 详情图Path列表（第一张为首图） |
| FileDetailUrlList | array string | 否 | 详情图Url列表（第一张为首图） |
| SkuList | array object | 否 | 商品规格Sku列表 |
| OnSaleStatus | int | 是 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |
| IsClearStocks | int | 否 | 是否是清货款：0否，1是 |
| FirstOnSaleDate | string | 否 | 最早上架时间 |
| FirstOnSalePerson | object | 否 | 最早上架人实体（简） |
| LastOnSaleDate | string | 否 | 最近上架时间 |
| LastOnSalePerson | object | 否 | 最近上架人实体（简） |
| LastOffShelvesDate | string | 否 | 最近下架时间 |
| LastOffShelvesPerson | object | 否 | 最近下架人实体（简） |
| SpecGroup | object | 否 | 规格组（说明见“获取规格模板列表”） |
| UnitList | array object | 否 | 计量单位列表（说明见通用） |
| TagList | array object | 否 | 标签列表（说明见通用） |
| BrandList | array object | 否 | 品牌列表（说明见通用） |
| SupplierList | array object | 否 | 供应商列表（说明见组织） |
| PriceGroupList | array object | 否 | 价格组列表（说明见通用） |
| ProductInventory | object | 否 | 库存（说明见仓储） |
| PriceRuleType | int | 否 | 定价规则：0按款定价，1按规格定价 |
| Price | object | 否 | 价格实体 |
| IsCreator | int | 否 | 商品是否属于自己：0否，1是 |
| ProductServiceType | int | 否 | 服务方式：0物流配送，1到店消费 |
| IsDisableRMA | int | 否 | 是否禁用退货：0否，1是 |
| CommissionRate | decimal\(18,4\) | 否 | 佣金比例 |
| EffectiveType | int | 否 | 有效类型：0天数，1日期 |
| EffectiveDays | int | 否 | 有效天数 |
| EffectiveDate | string | 否 | 有效期 |
|IsHidden|int | 否 | 是否隐藏 |

> #### Price说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CostPrice | decimal\(18,2\) | 否 | 成本价 |
| MarketPrice | decimal\(18,2\) | 否 | 市场价 |
| SalePrice | decimal\(18,2\) | 否 | 销售价 |
| MaxSalePrice | decimal\(18,2\) | 否 | 最大销售价 |

> #### SKU基础字段 {#请求数据}
>
> #### ProductGroup统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuCount | int | 否 | sku数量 |

> #### SKU基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | sku系统编码 |
| SkuName | string | 是 | sku名称 |
| SkuCode | string | 是 | sku代码 |
| SkuDetail | string | 否 | 详情 |
| SkuMemo | string | 否 | 备注 |
| BarCode | string | 否 | 条形码 |
| InternationalCode | string | 否 | 国际码 |
| GoodsWeight | decimal\(18,2\) | 否 | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否 | 体积 |
| SpecValueList | array object | 否 | 规格值列表 |
| IsClearStocks | int | 否 | 是否限制库存：0否，1是 |
| PriceGroupList | array object | 否 | 价格组列表（说明见通用） |
| SkuInventory | object | 否 | sku库存 |
| Price | object | 否 | 价格实体 |
| FileThumbnailUrlList | array string | 否 | 缩略图Url列表 |
| FileMasterUrlList | array string | 否 | 主图Url列表 |
| FileDetailUrlList | array string | 否 | 详情图Url列表 |
| ProductGroup | object | 否 | 款实体对象（不含SKU） |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围编码列表（店铺树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称\规格\标签） |
| ProductGroupClassSysNoList | array int | 否 | 类型分类系统编码（类别树） |
| OnSaleStatusList | array int | 否 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |
| TouristOrganizationSysNo | int | 否 | 游客组织系统编码（传0即为游客） |
| TagSysNoLIst | array int | 否 | 标签系统编码列表 |
| IsTagProduct | int | 否 | 是否显示含有标签的商品 |
|IsHidden|int | 否 | 是否隐藏 |
> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileThumbnailUrlList | int | 否 | 是否显示缩略图列表（数量） |
| IsShowFileMasterUrlList | int | 否 | 是否显示主图列表（数量） |
| IsShowFileDetailUrlList | int | 否 | 是否显示详情图列表（数量） |
| IsShowUnitList | int | 否 | 是否显示计量单位列表 |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowBrandList | int | 否 | 是否显示品牌列表 |
| IsShowSupplierList | int | 否 | 是否显示供应商列表 |
| IsShowSkuList | int | 否 | 是否显示sku列表 |
| IsShowSpecGroup | int | 否 | 是否显示规格组（说明见“获取规格模板列表”） |
| IsShowSpecValueList | int | 否 | 是否显示规格值（当IsShowSkuList/IsShowSpecGroup=1时启用） |
| ShowPriceGroupTypeList | array int | 否 | 价格组类型（见通用价格） |
| ShowPriceTypeList | array int | 否 | 价格类型（见通用价格） |
| IsShowProductInventory | int | 否 | 是否显示款库存（需要SKU库存则IsShowSkuInventory=1） |
| IsShowSkuInventory | int | 否 | 是否显示sku库存 |
| IsShowProductInSku | int | 否 | 是否显示sku中款的信息（款的图片需limit控制） |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1600101 | 商品模块 | 普通商品 |  | 新增页 |
| 1600102 |  | 普通商品 |  | 修改页 |
| 1600103 |  | 普通商品 |  | 详情页 |
| 1600104 |  | 普通商品 |  | 列表页 |



