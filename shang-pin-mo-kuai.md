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
| IsHidden | int | 否 | 是否隐藏 |
| IsSupportPointPay | int | 否 | 是否支持积分支付 |
| RewardPoint | int | 否 | 奖励积分 |
| ServiceType | int | 否 | 消费方式（0按次数，1按时间） |
| ServiceOutMinutes | int | 否 | 过期时间（分钟）（0为长期有效） |
| GroupList | array object | 否 | 商品组 |
| SortNo | int | 否 | 排序 |
| CPSCategory | string | 否 | 三方CPS类别 |
| CPSMaterialUrl | string | 否 | 三方CPSURL |
| CPSStartDate | string | 否 | 三方CPS开始推荐 |
| CPSEndDate | string | 否 | 三方CPS结束推荐 |
| CPSInOrderCount | int | 否 | 三方CPS评价 |
| FakeInventoryCount | int | 否 | 可砍份数 |
| IsTop | int | 是 | 是否置顶 |
| RewardMP | decimal | 否 | 奖励魔力 |
| FakeSaleCount | int | 是 | 虚假销量 |
| CPSMaterialUrl | string | 是 | CPS落地页 |
| CPSSysNo | int | 否 | CPS编码 |
| CPSCode | string | 否 | CPS编码 |
| SourceCPSSysNo | int | 是 | 来源三方CPS |
| SourceCPSName | string | 是 | 来源跳转三方名称 |
| CPSCommissionRate | int | 否 | 佣金比率 |
| CPSCommission | int | 否 | 佣金 |
| SourceProductGroupCode | string | 是 | 来源三方编码 |
| TaoWord | string | 是 | 淘口令 |
| SellerName | int | 是 | 商家名称 |
| StartSaleDate| datetime| 是 | 开卖时间|
| GroupByCode| string| 否 | 多款聚合款号 |
| IsGroupByDefault| int | 否 | 多款聚合默认显示 |
| GroupByOtherName| string| 否 | 多款聚合别名 |
| HollowSortNo | int | 否 | 坑位排序 |
| ShopShowSourceList|array[int] | 否 |展示来源（0普通，1蓝晶兑换） |
| LimitBuyCount | int | 否 | 限购数|
| IsAllSubsidyMP | int | 否 | 无论商品购买多少个，补贴魔力只给1份|
| IsLimitSubsidyMP | int | 否 | 限购魔力锁|
| LimitSubsidyMPStart | datetime | 否 | 限购魔力锁开始时间|
| LimitSubsidyMPEnd | datetime | 否 | 限购魔力锁结束时间|
| LimitSubsidyMPCount | int | 否 | 限购魔力锁最大份数|
| IsLockOnSaleStatus | int | 否 | 是否锁定上下架状态 |
| SubsidyMPLimitNewPerson | int | 否 | 补贴魔力是否只给新人（1是 0否）|
| NoCPSCode | string | 否 | 除三方来源编号 |
| BasicCommissionRate| decimal\(18,2\) | 否 |自购佣金比例 |

> #### Price说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CostPrice | decimal\(18,2\) | 否 | 成本价（桃子乐彩批发价） |
| MarketPrice | decimal\(18,2\) | 否 | 市场价（指导价） |
| SalePrice | decimal\(18,2\) | 否 | 销售价 |
| MaxSalePrice | decimal\(18,2\) | 否 | 最大销售价 |
| PointPrice | decimal\(18,2\) | 否 | 积分价格 |
| MinCutSalePrice | decimal\(18,2\) | 否 | 最低砍价 |
| OneBuyCutPrice | decimal\(18,2\) | 否 | 一元购必砍价 |
| CouponPrice| decimal\(18,2\) | 否 | 优惠券金额 |
| ReturnPrice | decimal\(18,2\) | 否 | 返还金额 |
| LJPrice | decimal\(18,2\) | 否 | 蓝晶价 |
|GrossProfit | decimal\(18,2\) | 否 |毛率利 |


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
| CPSCommissionRate | int | 否 | 佣金比率 |
| CPSCommission | int | 否 | 佣金 |
| OnSaleStatus | int | 否 | 上下架状态 0待上架 1上架 2下架 |
| IsHidden | int | 是 | 是否屏蔽|
| DeliveryPlace| string | 是 | 发货地|
| MinQuantity| int | 否 | 起订数量 |
| LimitQuantity| int | 否 | 限购数量 |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> ### SkuInventory

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | 商品规格\(SKU\)系统编码 |
| PhysicalQuantity | int | 是 | 物理库存 |
| AvailableQuantity | int | 是 | 可用库存 |
| VirtualQuantity | int | 是 | 虚拟库存 |
| FrozenQuantity | int | 是 | 冻结库存（含冻结库位库存+不可用库位库存+次品） |
| OrderLockQuantity | int | 是 | 订单锁数量 |
| DeliveryVoucherLockQuantity | int | 是 | 发货单锁数量 |

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
| NotInTagSysNoLIst | array int | 否 | 不在标签系统编码列表 |
| IsTagProduct | int | 否 | 是否显示含有标签的商品 |
| IsHidden | int | 否 | 是否隐藏 |
| ShopPCDCode | string | 否 | 店铺PCD代码 |
| ShopPCDDescription | string | 否 | 店铺PCD描述 |
| IndustryClassSysNoList | array int | 否 | 行业类别 |
| IsSupportPointPay | int | 否 | 是否支持积分支付 |
| GroupSysNo | int | 否 | 商品组系统编码 |
| ShopShowSource | int | 否 | 店铺展示位置 |
| ProductGroupCode | string | 否 | 款号 |
| CPSCode | string | 是 | CPS名称 JD京东，YX严选 |
| BrandSysNoList | array int | 否 | 品牌系统编码列表 |
| ProductServiceTypeList | array int | 否 | 服务方式：0物流配送，1到店消费 |
| StartLastOnSaleDate | string | 否 | 开始最近上架时间 |
| EndLastOnSaleDate | string | 否 | 终止最近上架时间 |
| StartCPSEndDate | string | 否 | 开始三方CPS结束推荐 |
| EndCPSEndDate | string | 否 | 终止三方CPS结束推荐 |
| SellerName | string | 是 | 商家名称 |
| GroupByCode| string| 否 | 多款聚合款号 |
| HollowSysNo | int | 是 | 坑位编码 |
| ShopShowSourceList|array[int] | 否 |款展示来源（0普通，1蓝晶兑换） |
| StartBasicCommissionRate| decimal\(18,2\) | 否 |起始自购佣金比例 |
| EndBasicCommissionRate| decimal\(18,2\) | 否 |终止自购佣金比例 |
| StartCPSCommissionRate | int | 否 | 起始佣金比率 |
| EndCPSCommissionRate | int | 否 | 终止佣金比率 |

#### SpecGroup

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecGroupSysNo | int | 是 | 规格组系统编码 |
| SpecGroupName | string | 是 | 规格组名称 |
| SpecList | array object | 是 | 规格列表 |

#### Spec {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecSysNo | int | 是 | 规格系统编码 |
| SpecName | string | 是 | 规格名称 |
| SpecValueList | array object | 是 | 规格值列表 |

#### SpecValue {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecValueSysNo | int | 是 | 规格值系统编码 |
| SpecName | string | 是 | 规格名称 |
| SpecValue | string | 是 | 规格值 |
| SpecValueOtherName | string | 否 | 规格值别名 |
| IsCustomized | int | 是 | 是否可定制：0否，1是 |
| IsChecked | int | 否 | 是否选中：0否，1是 |
| IconColor | string | 否 | 色号 |
| SpecValueFee | decimal\(18,2\) | 否 | 费用 |
| SpecValueUrlList | array string | 否 | 图片 |

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
| IsShowGroupList | int | 否 | 是否显示商品组 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1600101 | 商品模块 | 普通商品 |  | 新增页 |
| 1600102 |  | 普通商品 |  | 修改页 |
| 1600103 |  | 普通商品 |  | 详情页 |
| 1600104 |  | 普通商品 |  | 列表页 |



