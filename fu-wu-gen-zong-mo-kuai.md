# 服务跟踪模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackSysNo | int | 是 | 系统编码 |
| TrackType | int | 是 | 类型（枚举） |
| TrackClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| TrackClassName | string | 否 | 分类名称 |
| TrackTitle | string | 是 | 标题 |
| TrackContent | string | 是 | 内容 |
| TrackTime | string | 否 | 时间 |
| TrackStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| RemovePersonSysNo | int | 否 | 撤下人员编码 |
| RemoveTime | string | 否 | 撤下时间 |
| PublishPerson | object | 否 | 发布人员实体对象 |
| RemovePerson | object | 否 | 撤下人员实体对象 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| IsNeedMoments | int | 否 | 是否需要关联朋友圈 |
| IsPublic | int | 否 | 是否公开 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| PointsValueList | array object | 否 | 积分赠送配置值列表（接口） |
| ModuleRelationList | array object | 否 | 关联模块列表 |

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
| PersonSysNo | int | 否 | 人员编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| TrackStartTime | string | 否 | 开始时间 |
| TrackEndTime | string | 否 | 结束时间 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowModuleRelationList | int | 否 | 是否显示关联模块列表 |
| IsShowMomentsUrlList | int | 否 | 是否显示朋友圈图片列表（该参数即返回数量） |

#### ModuleRelationList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1400101 | 服务跟踪模块 | 服务承诺 |  | 新增页 |
| 1400102 |  | 服务承诺 |  | 修改页 |
| 1400103 |  | 服务承诺 |  | 详情页 |
| 1400104 |  | 服务承诺 |  | 列表页 |



