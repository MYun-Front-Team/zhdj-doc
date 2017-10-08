# 活动模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |
| ActivityType | int | 是 | 类型（枚举） |
| ActivityClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| ActivityClassName | string | 否 | 分类名称 |
| ActivityTitle | string | 是 | 标题 |
| ActivityContent | string | 是 | 内容 |
| ActivityStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| RemovePersonSysNo | int | 否 | 撤下人员编码 |
| RemoveTime | string | 否 | 撤下时间 |
| PublishPerson | object | 否 | 发布人员实体对象 |
| RemovePerson | object | 否 | 撤下人员实体对象 |
| MaxPersonNum | int | 是 | 人数上限（0无限） |
| ActivitySignUpStartTime | string | 是 | 报名开始时间 |
| ActivitySignUpEndTime | string | 是 | 报名结束时间 |
| ActivityStartTime | string | 是 | 活动开始时间 |
| ActivityEndTime | string | 是 | 活动结束时间 |
| ActivityPlace | string | 是 | 活动地点 |
| ActivitySummary | string | 否 | 活动记要 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| IsNeedMoments | int | 否 | 是否需要关联朋友圈 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| PointsValueList | array object | 否 | 积分赠送配置值列表（接口） |
| ActivityPersonList | array object | 否 | 人员足迹列表 |
| ModuleRelationList | array object | 否 | 关联模块列表 |
| HostPersonSysNo | int | 否 | 主持人编码 |
| HostPersonName | string | 否 | 主持人姓名 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignUpCount | int | 否 | 报名人数 |
| SignInCount | int | 否 | 签到人数 |
| LeaveCount | int | 否 | 请假人数 |
| ReportCount | int | 否 | 汇报人员（个人记要不为空） |
| ActivityInstantStatus | int | 是 | 活动即时状态：1未开始，2进行中，3已结束 |
| ActivitySignUpStatus | int | 是 | 活动报名即时状态：1未开始，2进行中，3已结束 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddActivity | 操作 | 是 | 新增 |
| EditActivity | 操作 | 是 | 修改 |
| DeleteActivity | 操作 | 是 | 删除 |
| PublishActivity | 操作 | 是 | 发布 |
| RemoveActivity | 操作 | 否 | 撤下 |
| SignUpActivity | 操作 | 是 | 报名 |
| SignInActivity | 操作 | 否 | 签到 |
| LeaveActivity | 操作 | 否 | 请假 |
| SaveActivitySummary | 操作 | 否 | 修改活动记要 |
| SaveActivityPersonSummary | 操作 | 否 | 修改活动个人记要 |
| GetActivityFieldListByPage | 查询 | 是 | 根据页面，获取可选字段列表 |
| GetActivityList | 搜索 | 是 | 搜索列表 |
| GetActivityBySysNo | 查询 | 是 | 根据编码，获取详情 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题、地点） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowPointsValueList | int | 否 | 是否显示积分配置列表 |
| ~~IsShowActivityPersonList~~ | ~~int~~ | ~~否~~ | ~~是否显示人员列表~~ |
| IsShowModuleRelationList | int | 否 | 是否显示模块关联列表 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况 |
| IsShowReportList | int | 否 | 是否显示汇报列表 |

#### ActivityPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityPersonSysNo | int | 是 | 人员足迹系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| ActivityPersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：0参会人员，1报名, 10签到，11请假，12缺席 |
| SignUpTime | string | 是 | 报名时间 |
| SignTime | string | 否 | 签到时间 |
| SignPlace | string | 否 | 签到地点（定位） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Reason | string | 否 | 请假原因 |
| ~~SignSummary~~ | ~~string~~ | ~~否~~ | ~~个人记要~~ |
| ~~SignSummaryTime~~ | ~~string~~ | ~~否~~ | ~~个人记要时间~~ |
| Remark | string | 否 | 备注 |

#### ModuleRelationList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceType | int | 否 | 关联模块类型 |
| ModuleSourceClass | int | 否 | 关联模块分类 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |
| ModuleSourceTitle | string | 否 | 关联模块主题 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 400101 | 活动模块 | 主题党日 |  | 新增页 |
| 400102 |  | 主题党日 |  | 修改页 |
| 400103 |  | 主题党日 |  | 详情页 |
| 400104 |  | 主题党日 |  | 列表页 |
| 400201 |  | 三会一课 |  | 新增页 |
| 400202 |  | 三会一课 |  | 修改页 |
| 400203 |  | 三会一课 |  | 详情页 |
| 400204 |  | 三会一课 |  | 列表页 |



