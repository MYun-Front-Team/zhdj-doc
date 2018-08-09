# 店铺模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码（店铺树） |
| ShopSysNo | int | 是 | 店铺系统编码 |
| ShopType | int | 是 | 类型（枚举） |
| ShopClassSysNo | int | 否 | 类别系统编码（分类树） |
| ShopClassName | int | 否 | 类别名称 |
| ShopName | string | 是 | 店铺名称 |
| ShopShortName | string | 否 | 店铺简称 |
| ShopTel | string | 否 | 店铺联系电话 |
| ShopDesc | string | 否 | 店铺描述 |
| ShopMaster | string | 否 | 店铺负责人 |
| ShopPost | string | 否 | 店铺负责人岗位 |
| ShopPerson | string | 否 | 店铺联系人 |
| ShopPersonPhone | string | 否 | 店铺联系人电话 |
| ShopPersonPost | string | 否 | 店铺联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| OpenStatus | int | 是 | 开店状态：0待装修，10开，11关 |
| OpenTime | string | 否 | 开店时间 |
| BusinessStartTime | string | 否 | 营业开始时间 |
| BusinessEndTime | string | 否 | 营业结束时间 |
| ServiceStartTime | string | 否 | 客服服务开始时间 |
| ServiceEndTime | string | 否 | 客服服务结束时间 |
| ShopLogoPathList | array string | 否 | 店铺Logo的Path路径列表 |
| ShopLogoUrlList | array string | 否 | 店铺Logo的Url路径列表 |
| ShopNo | string | 否 | 店铺编号 |
| ShopUsedStatus | int | 否 | 店铺使用状态：0闲置，10使用 |
| ShopArea | decimal\(18,2\) | 否 | 店铺面积（平方） |
| ShopPropertyFee | decimal\(18,2\) | 否 | 店铺物业费（元/年） |
| ShopDepositFee | decimal\(18,2\) | 否 | 店铺默认押金（元） |
| ShopRentFee | decimal\(18,2\) | 否 | 店铺默认租金（元/月） |
| ShopRentRemark | string | 否 | 店铺租用备注 |
| ShopCategoryList | array object | 否 | 店铺主营分类列表（行业） |
| ShopLease | object | 否 | 店铺最近租用记录 |
| IsCertified | int | 否 | 是否认证：0否，1是 |
| ProductGroupList | array object | 否 | 店铺推荐商品列表 |
| Brand | object | 否 | 品牌 |
| ShopCommission | decimal\(18,4\) | 否 | 店铺佣金 |
| RmaAddress | string | 否 | 退货地址 |
| ShopBannerPathList | array string | 否 | 店铺Banner路径列表 |
| ShopBannerUrlList | array string | 否 | 店铺Banner的URL列表 |
| StarsRemark| decimal | 否 | 店铺星级 |
| ContractPCDCode| string | 否 | 联系地址 |
| ContractPCDDescription| string | 否 | 联系地址 |
| SortNo | int | 否 | 排序 |
| ShopShowSourceSysNos|array[int] | 否 | 店铺展示位置 |
| IsScanCode| int | 否 | 是否有扫码功能 |
| RecruitNeedAudit| int | 否 |发布岗位是否要审核（1要，0不要） |
| IsAuthentication| int | 否 | 发岗位是否认证 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| PositionUrlList | array string | 否 | 工作地Path文件列表 |
| Seller| Seller| 否 | 验证商家信息 |




> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupCount | int | 否 | 商品数量 |
| PersonFollowCount | int | 否 | 关注数量 |
| DeviceCount | int | 否 | 设备数量 |
|SalePersonCount|int | 否 |消费人数 |
|Wallet|int | 否 |钱包|

### Seller

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| SellerName | string | 是 | 商家名称 |



> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表（店铺树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| ShopUsedStatusList | array int | 否 | 店铺使用状态：0闲置，10使用 |
| ShopClassSysNoList | array int | 否 | 类别系统编码（分类树） |
| IsCertified | int | 否 | 是否认证 |
| CategorySysNoList | array int | 否 | 主营分类（行业） |
| BrandSysNoList | array int | 否 | 品牌系统编码 |
| Longitude | decimal\(18,10\) | 否 | 经度 |
| Latitude | decimal\(18,10\) | 否 | 纬度 |
| ContractPCDCode| string | 否 | 联系地址 |
| ContractPCDDescription| string | 否 | 联系地址 |
| ShopShowSource|int | 否 | 店铺展示位置 |
|OpenStatusList | array int | 否 |开店状态：0待装修，10开，11关 |


> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowProductGroupCount | int | 否 | 是否显示商品数量 |
| IsShowPersonFollowCount | int | 否 | 是否显示关注数量 |
| IsShowShopCategoryList | int | 否 | 是否显示主营分类列表 |
| IsShowDeviceCount | int | 否 | 是否显示设备数量 |
| IsShowShopLease | int | 否 | 是否显示店铺最近租用记录 |
| IsShowProductGroupList | int | 否 | 是否显示推荐商品（值为显示的数量） |
| IsShowBrand | int | 否 | 是否显示品牌 |
| IsShowShopBannerUrlList | int | 否 | 是否显示店铺Banner列表 |
| IsShowWallet| int | 否 | 是否显示钱包|


####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1500100 | 店铺模块 |  |  | 店铺首页 |
| 1500101 |  |  |  | 新增页 |
| 1500102 |  |  |  | 修改页 |
| 1500103 |  |  |  | 详情页 |
| 1500104 |  |  |  | 列表页 |



