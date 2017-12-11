# 工单模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 | 系统编码 |
| WorkType | int | 是 | 类型（枚举） |
| WorkClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| WorkClassName | string | 否 | 分类名称 |
| WorkTitle | string | 是 | 标题 |
| WorkContent | string | 是 | 内容 |
| WorkTime | string | 否 | 发生时间 |
| WorkStatus | int | 是 | 状态：0待处理，10已处理 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| WorkAddress | string | 否 | 发生地地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| FromPerson | object | 否 | 发布人员实体对象 |
| ToPerson | object | 否 | 处理人员实体对象 |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| TagList | array object | 否 | 标签列表（见通用-标签） |
| CommentList | array object | 否 | 评价列表（见通用-评价） |
| ReplyList | array object | 否 | 回复列表 |

> #### Reply说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FromPerson | object | 是 | 处理人实体（简版） |
| FromDataRange | object | 是 | 处理人所属数据范围结点 |
| ReplySysNo | int | 是 | 回复系统编码 |
| ReplyContent | string | 是 | 回复内容 |
| ReplyTime | string | 是 | 回复时间 |
| ReplyType | int | 是 | 回复类型：0回复，1流转 |
| ToPerson | object | 否 | 流转人实体（当类型为流转时存在） |
| ToDataRange | object | 否 | 流转人所属数据范围结点（当类型为流转时存在） |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| FromPersonSysNo | int | 否 | 上报人员人员编码 |
| ToPersonSysNo | int | 否 | 处理人员系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题/内容） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| IsMyDealPrint | int | 否 | 是否显示自己待处理的：0否，1是 |
| WorkStartTime | string | 否 | 开始时间 |
| WorkEndTime | string | 否 | 结束时间 |
| WorkStatusList | array int | 否 | 状态：0待处理，10已处理 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowCommentList | int | 否 | 是否显示评论列表 |
| IsShowReplyList | int | 否 | 是否显示回复列表 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 2400101 | 工单模块 | 民情民意 |  | 新增页 |
| 2400102 |  | 民情民意 |  | 修改页 |
| 2400103 |  | 民情民意 |  | 详情页 |
| 2400104 |  | 民情民意 |  | 列表页 |



