# 设备模块-字段说明 {#新增河流}

> #### Equipment基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备系统编码 |
| OrganizationSysNo | int | 是 | 产权所属组织系统编码 |
| OrganizationName | string | 是 | 产权所属组织 |
| DataRangeSysNo | int | 是 | 数据范围编码列表 |
| DataRangeName | string | 是 | 数据范围名称 |
| PersonSysNo | int | 是 | 产权人编码 |
| PersonName | string | 是 | 产权人姓名 |
| CellPhoneNo | string | 是 | 产权人手机 |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| Passageway | int | 是 | 货道数量 |
| SN | string | 是 | SN号 |
| EquipmentName | string | 是 | 设备名称 |
| PCDCode | string | 是 | PCD代码 |
| PCDDescription | string | 是 | PCD描述 |
| Location | string | 是 | 具体位置 |
| QCCode | string | 是 | 二维码 |
| EquipmentStatus | int | 是 | 设备状态10正常 11故障 |
| OnlineStatus | int | 是 | 在线状态10在线 11离线 |
| FaultType | string | 否 | 故障类型描述 |
| FaultTime | datetime | 否 | 故障时间 |
| LineSysNo | int | 否 | 线路编码 |
| LineName | string | 否 | 线路名称 |
| PassagewayList | array object | 否 | 货道商品列表 |
|  |  |  |  |

**Passageway货道商品**

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EquipmentSysNo | int | 是 | 设备编码 |
| PassagewayNo | int | 是 | 货道号 |
| ProductGroupSysNo | int | 是 | 商品编码 |
| ProductGroupName | string | 是 | 商品名称 |
| ImgList | array string | 是 | 图片列表 |
| SalePrice | decimal\(18,2\) | 是 | 销售价格 |
| OutStock | int | 是 | 10正常，11缺货 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 产权人组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围编码列表 |
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



