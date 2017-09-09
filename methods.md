# 活动模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |
| ActivityType | int | 是 | 类型（枚举） |
| ActivityClassSysNo | int | 是 | 类型分类系统编码（类别树） |
| ActivityTitle | string | 是 | 标题 |
| ActivityContent | string | 是 | 内容 |
| ActivityStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| RemovePersonSysNo | int | 否 | 撤下人员编码 |
| RemoveTime | string | 否 | 撤下时间 |
| PublishPerson | array | 否 | 发布人员实体对象 |
| RemovePerson | array | 否 | 撤下人员实体对象 |
| MaxPersonNum | int | 是 | 人数上限（0无限） |
| ActivitySignUpStartTime | string | 是 | 报名开始时间 |
| ActivitySignUpEndTime | string | 是 | 报名结束时间 |
| ActivityStartTime | string | 是 | 活动开始时间 |
| ActivityEndTime | string | 是 | 活动结束时间 |
| ActivityPlace | string | 是 | 活动地点 |
| ActivitySummary | string | 否 | 活动记要 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| PointsValueList | array object | 否 | 积分赠送配置值列表 |
| ActivityPersonList | array object | 否 | 人员列表 |
| IsNeedMoments | int | 否 | 是否需要关联朋友圈 |

> #### 统计字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignUpCount | int | 否 | 报名人数 |
| SignInCount | int | 否 | 签到人数 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddActivity | 操作 | 是 | 新增 |
| EditActivity | 操作 | 是 | 修改 |
| PublishActivity | 操作 | 是 | 发布 |
| RemoveActivity | 操作 | 否 | 撤下 |
| SignUpActivity | 操作 | 是 | 报名 |
| SignInActivity | 操作 | 否 | 签到 |
| LeaveActivity | 操作 | 否 | 请假 |
| SaveActivitySummary | 操作 | 否 | 修改记要 |
|  |  |  |  |
| GetActivityList | 搜索 | 是 | 搜索列表 |
| GetActivityBySysNo | 查询 | 是 | 根据编码，获取详情 |



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| IsMerge | int | 否 | 是否向下兼容查询 |
|  |  |  |  |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowPointsValueList | int | 否 | 是否显示积分配置列表 |
| IsShowActivityPersonList | int | 否 | 是否显示人员列表 |
| IsShowMoments | int | 否 | 是否显示朋友圈模块 |
|  |  |  |  |



