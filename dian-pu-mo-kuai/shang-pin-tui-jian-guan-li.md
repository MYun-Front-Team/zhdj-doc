# 商品推荐管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 推荐组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（推荐位置树） |
| RecommendSysNo | int | 是 | 推荐系统编码 |
| RecommendType | int | 是 | 类型：0首页推荐，1特惠 |
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

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendStatus | int | 否 | 推荐状态：0未开始，1进行中，2已过期 |

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
| RecommendStatusList | array int | 否 | 推荐状态：0未开始，1进行中，2已过期 |
| RecommendTypeList | array int | 否 | 推荐类型 |
| AreaSysNo | int | 否 | 推荐区域系统编码 |
| CategorySysNo | int | 否 | 推荐行业系统编码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowSeller | int | 否 | 是否显示商家 |
| IsShowShop | int | 否 | 是否显示店铺 |
| IsShowHollowTime | int | 否 | 是否启用坑位时间（一旦启用，那么当前时间必须在启用时间范围内，适用前台） |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



