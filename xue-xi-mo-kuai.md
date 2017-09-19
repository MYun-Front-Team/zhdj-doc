# 学习模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudySysNo | int | 是 | 系统编码 |
| StudyType | int | 是 | 类型（枚举） |
| StudyClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| StudyClassName | string | 否 | 分类名称 |
| StudyTitle | string | 是 | 标题 |
| StudyContent | string | 是 | 内容 |
| StudyStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| RemovePersonSysNo | int | 否 | 撤下人员编码 |
| RemoveTime | string | 否 | 撤下时间 |
| PublishPerson | object | 否 | 发布人员实体对象 |
| RemovePerson | object | 否 | 撤下人员实体对象 |
| StudyStartTime | string | 否 | 学习开始时间 |
| StudyEndTime | string | 否 | 学习结束时间 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| IsNeedMoments | int | 否 | 是否需要关联朋友圈 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| PointsValueList | array object | 否 | 积分赠送配置值列表（接口） |
| StudyPersonList | array object | 否 | 人员足迹列表 |
| ModuleRelationList | array object | 否 | 关联模块列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudyCount | int | 否 | 学习（浏览）人数 |
| UploadCount | int | 否 | 上传人数 |
| ReportCount | int | 否 | 汇报人数 |
| StudyStatus | int | 否 | 学习即时状态：1未开始，2进行中，3已结束 |
| MyStudyStatus | int | 否 | 当前浏览人的查看状态：0未阅，1已阅 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddStudy | 操作 | 是 | 新增 |
| EditStudy | 操作 | 是 | 修改 |
| DeleteStudy | 操作 | 是 | 删除 |
| PublishStudy | 操作 | 是 | 发布 |
| RemoveStudy | 操作 | 是 | 撤下 |
| SetLookingAlway | 操作 | 是 | 心跳保活 |
| GetStudyFieldListByPage | 查询 | 是 | 根据页面，获取可选字段列表 |
| GetStudyList | 搜索 | 是 | 搜索列表 |
| GetStudyBySysNo | 查询 | 是 | 根据编码，获取详情 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题、地点） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowPointsValueList | int | 否 | 是否显示积分配置列表 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况（MyStudyStatus的开关） |

#### StudyPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudyPersonSysNo | int | 是 | 人员足迹系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| StudyPersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：3浏览 |
| SignStartTime | string | 是 | 学习开始时间 |
| StudySecond | int | 是 | 学习秒数 |
| IsLooking | int | 是 | 是否还在阅读 |
| Remark | string | 否 | 备注 |

#### ModuleRelationList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 800101 | 学习模块 | 两学一做 |  | 新增页 |
| 800102 |  | 两学一做 |  | 修改页 |
| 800103 |  | 两学一做 |  | 详情页 |
| 800104 |  | 两学一做 |  | 列表页 |
| 800201 |  | 红色e课堂 |  | 新增页 |
| 800202 |  | 红色e课堂 |  | 修改页 |
| 800203 |  | 红色e课堂 |  | 详情页 |
| 800204 |  | 红色e课堂 |  | 列表页 |



