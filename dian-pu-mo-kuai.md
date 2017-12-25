# 店铺模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码（店铺树） |
| ShopSysNo | int | 是 | 店铺系统编码 |
| ShopType | int | 是 | 类型（枚举） |
| ShopClassSysNo | int | 否 | 类别系统编码（分类树） |
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
| ShopCategoryList | array object | 否 | 店铺主营分类列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupCount | int | 否 | 商品数量 |
| PersonFollowCount | int | 否 | 关注数量 |

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

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowProductGroupCount | int | 否 | 是否显示商品数量 |
| IsShowPersonFollowCount | int | 否 | 是否显示关注数量 |
| IsShowShopCategoryList | int | 否 | 是否显示主营分类列表 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1500100 | 店铺模块 |  |  | 店铺首页 |
| 1500101 |  |  |  | 新增页 |
| 1500102 |  |  |  | 修改页 |
| 1500103 |  |  |  | 详情页 |
| 1500104 |  |  |  | 列表页 |



