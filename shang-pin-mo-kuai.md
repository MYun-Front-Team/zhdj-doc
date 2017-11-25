# 商品模块-字段说明 {#新增河流}

> #### ProductGroup基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |
| ProductGroupType | int | 是 | 类型（枚举） |
| ProductGroupClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| ProductGroupClassName | string | 否 | 分类名称 |
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
| PriceGroupList | array object | 否 | 价格组列表（说明见通用） |

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

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称\规格\标签） |
| ProductGroupClassSysNoList | array int | 否 | 类型分类系统编码（类别树） |
| OnSaleStatusList | array int | 否 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileThumbnailUrlList | int | 否 | 是否显示缩略图列表（数量） |
| IsShowFileMasterUrlList | int | 否 | 是否显示主图列表（数量） |
| IsShowUnitList | int | 否 | 是否显示计量单位列表 |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowSkuList | int | 否 | 是否显示sku列表 |
| IsShowSpecGroup | int | 否 | 是否显示规格组（说明见“获取规格模板列表”） |
| IsShowSpecValueList | int | 否 | 是否显示规格值（当IsShowSkuList/IsShowSpecGroup=1时启用） |
| ShowPriceGroupTypeList | array int | 否 | 价格组类型（见通用价格） |
| ShowPriceTypeList | array int | 否 | 价格类型（见通用价格） |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1600101 | 商品模块 | 普通商品 |  | 新增页 |
| 1600102 |  | 普通商品 |  | 修改页 |
| 1600103 |  | 普通商品 |  | 详情页 |
| 1600104 |  | 普通商品 |  | 列表页 |



