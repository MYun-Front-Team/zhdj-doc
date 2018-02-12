# 分润管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| VideoSysNo | int | 是 | 视频系统编码 |
| VideoTitle | string | 是 | 视频标题 |
| VideoStatus | int | 是 | 状态：0新建，10发布，11撤下 |
| IsShield | int | 是 | 是否屏蔽：0否，1是 |
| ShieldReason | string | 否 | 屏蔽理由 |
| VideoID | string | 否 | 第三方视频ID |
| Organization | object | 否 | 组织 |
| Seller | object | 否 | 商家 |
| VideoPathList | array string | 否 | 视频主图path路径 |
| VideoUrlList | array string | 否 | 视频主图url路径 |
| VideoPersonList | array object | 否 | 人员足迹列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BrowseCount | int | 否 | 浏览数量 |
| CollectCount | int | 否 | 收藏数量 |
| MyBrowseStatus | int | 否 | 我的浏览状态 |
| MyCollectStatus | int | 否 | 我的收藏数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| VideoStatusList | array int | 否 | 状态：0新建，10发布，11撤下 |
| IsShieldList | array int | 否 | 是否屏蔽：0否，1是 |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowSeller | int | 否 | 是否显示商家 |
| IsShowVideoUrlList | int | 否 | 是否显示主图列表 |
| IsShowBrowseCount | int | 否 | 是否显示浏览数量 |
| IsShowCollectCount | int | 否 | 是否显示收藏数量 |
| IsShowMyBrowseStatus | int | 否 | 是否显示我的浏览状态 |
| IsShowMyCollectStatus | int | 否 | 是否显示我的收藏数量 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



