# 坑位管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 投放组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（投放位置树） |
| DataRangeNames| array[string]| 是 | 数据范围系统名称（投放位置树：从祖先到自己） |
| HollowSysNo | int | 是 | 坑位系统编码 |
| HollowType | int | 是 | 坑位类型：0链接，1商品，2店铺，3新闻 |
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



> #### HollowObject {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| HollowUrl | string | 否 | 链接地址 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
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

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



