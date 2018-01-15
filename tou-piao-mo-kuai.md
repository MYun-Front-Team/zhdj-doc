# 投票模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 活动系统编码 |
| VoteType | int | 是 | 类型（枚举） |
| VoteClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| VoteClassName | string | 否 | 分类名称 |
| VoteTitle | string | 是 | 标题 |
| VoteContent | string | 是 | 内容 |
| VoteStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| RemovePersonSysNo | int | 否 | 撤下人员编码 |
| RemoveTime | string | 否 | 撤下时间 |
| PublishPerson | object | 否 | 发布人员实体对象 |
| RemovePerson | object | 否 | 撤下人员实体对象 |
| VoteStartTime | string | 是 | 报名开始时间 |
| VoteEndTime | string | 是 | 报名结束时间 |
| VoteSummary | string | 否 | 投票记要 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| PointsValueList | array object | 否 | 积分赠送配置值列表（接口） |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| Propertys | array object | 否 | 选项属性列表（见通用-属性） |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VotePersonCount | int | 否 | 应投票人员人数 |
| ViewCount | int | 否 | 已阅人数 |
| SignInCount | int | 否 | 投票人数 |
| LeaveCount | int | 否 | 弃票人数 |
| VoteSignUpStatus | int | 是 | 投票即时状态：1未开始，2进行中，3已结束 |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| VoteTypeList | array int | 否 | 投票类型（枚举） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题、地点） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPropertyFileUrlList | int | 否 | 是否显示属性文件图片列表 |
| IsShowPointsValueList | int | 否 | 是否显示积分配置列表 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况 |
| IsShowPropertys | int | 否 | 是否显示选项属性列表 |
| IsShowPropertyStatistics | int | 否 | 是否显示属性统计（IsShowPropertys=1时有效） |
| IsShowPropertySelected | int | 否 | 是否显示投票情况 |

#### VotePersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VotePersonSysNo | int | 是 | 人员足迹系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| VotePersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：0未投，1已阅, 10已投，11弃票 |
| SignTime | string | 否 | 投票时间 |
| Reason | string | 否 | 请假原因 |
| Remark | string | 否 | 备注 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 2900101 | 投票模块 | 业委会投票 |  | 新增页 |
| 2900102 |  | 业委会投票 |  | 修改页 |
| 2900103 |  | 业委会投票 |  | 详情页 |
| 2900104 |  | 业委会投票 |  | 列表页 |
|  |  |  |  |  |



