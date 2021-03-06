# 坑位管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 投放组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（投放位置树） |
| DataRangeNames| array[string]| 是 | 数据范围系统名称（投放位置树：从祖先到自己） |
| HollowSysNo | int | 是 | 坑位系统编码 |
| HollowType | int | 是 | 坑位类型：0链接，1商品，2店铺，3新闻,4录播,5消息,6活动，7商品推荐集合页 |
| LaunchCategorySysNo | int | 否 | 投放行业系统编码 |
| LaunchAreaSysNo | int | 否 | 投放区域系统编码 |
| LaunchPCDCode | string | 否 | 投放区域PCDCode |
| LaunchPCDDesc | string | 否 | 投放区域PCD描述 |
| HollowTitle | string | 是 | 坑位标题 |
| HollowContent | string | 否 | 坑位内容 |
| HollowStatus | int | 是 | 状态：0新建，10发布，11撤下 |
| HollowStartTime | string | 是 | 启用开始时间 |
| HollowEndTime | string | 是 | 启用结束时间 |
| Remark | string | 否 | 备注 |
| PublishTime | string | 否 | 发布时间 |
| PublishPerson | object | 否 | 发布人 |
| RemoveTime | string | 否 | 撤下时间 |
| RemovePerson | object | 否 | 撤下人 |
| IsShield | int | 否 | 是否屏蔽：0否，1是 |
| ShieldReason | string | 否 | 屏蔽原因 |
| Organization | object | 否 | 组织 |
| Seller | object | 否 | 商家 |
| HollowPathList | array string | 否 | 坑位主图path路径 |
| HollowUrlList | array string | 否 | 坑位主图url路径 |
| HollowObjectList | array object | 否 | 坑位中对象实体列表 |
| HollowLogoPathList | array string | 否 | 坑位LOGOpath路径 |
| HollowLogoUrlList | array string | 否 | 坑位LOGOurl路径 |
| HollowBackPathList | array string | 否 | 坑位背景path路径 |
| HollowBackUrlList | array string | 否 | 坑位背景url路径 |
| SortNo| int | 是 | 排序 |
| BackColor | string | 否 |背景色 |




> #### HollowObject {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| ModuleSourceName| string | 否 | 来源系统名称 |
| HollowUrl | string | 否 | 链接地址 |
| OrganizationSysNo | int | 是 | 商品组织系统编码 |
| Price| Price| 否 | 价格（商品有效） |
| ModuleFileThumbnailUrlList | array string | 否 | 缩略图列表 |
| FakeSaleCount|int| 是 |销售数（商品有效） |
| FakeInventoryCount|int| 是 |假库存数（商品有效） |





> #### Price说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CostPrice | decimal\(18,2\) | 否 | 成本价 |
| MarketPrice | decimal\(18,2\) | 否 | 市场价 |
| SalePrice | decimal\(18,2\) | 否 | 销售价 |
| MaxSalePrice | decimal\(18,2\) | 否 | 最大销售价 |
| PointPrice | decimal\(18,2\) | 否 | 积分价格 |
| MinCutSalePrice | decimal\(18,2\) | 否 | 最低砍价 |
| OneBuyCutPrice | decimal\(18,2\) | 否 | 一元购必砍价 |
| CouponPrice| decimal\(18,2\) | 否 | 优惠券金额 |
| ReturnPrice | decimal\(18,2\) | 否 | 返还金额 |





> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ObjectCount | int | 否 | 对象数量 |
| BrowseCount | int | 否 | 浏览数量 |
| VisitorCount | int | 否 | 浏览人次 |
| LaunchStatus | int | 否 | 投放状态：0未开始，1进行中，2已过期（只有当已发布状态时该值有意义） |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围系统编码（投放位置树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| HollowStatusList | array int | 否 | 状态：0新建，10发布，11撤下 |
| HollowTypeList | array int | 否 | 坑位类型 |
| IsShieldList | array int | 否 | 是否屏蔽：0否，1是 |
| LaunchAreaSysNo | int | 否 | 投放区域系统编码 |
| LaunchCategorySysNo | int | 否 | 投放行业系统编码 |
| LaunchPCDDesc | string| 否 |投放区域PCD描述  |
| LaunchStatusList| array object | 否 |投放状态：0未开始，1进行中，2已过期（只有当已发布状态时该值有意义） |
|DataRangeCodeList| array string| 否 |投放位置编码 |


> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowSeller | int | 否 | 是否显示商家 |
| IsShowHollowUrlList | int | 否 | 是否显示主图列表 |
| IsShowBrowseCount | int | 否 | 是否显示浏览数量 |
| IsShowVisitorCount | int | 否 | 是否显示浏览人次 |
| IsShowHollowObjectList | int | 否 | 是否显示坑位中对象实体列表 |
| IsShowHollowTime | int | 否 | 是否启用坑位时间（一旦启用，那么当前时间必须在启用时间范围内，适用前台） |
| IsShowHollowObjectFile | int | 否 | 是否显示坑位中对象实体图片 |
| IsShowHollowObjectPrice| int | 否 | 是否显示坑位中对象实体价格 |




####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



