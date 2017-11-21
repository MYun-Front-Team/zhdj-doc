# 新闻模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsSysNo | int | 是 | 系统编码 |
| NewsType | int | 是 | 类型（枚举） |
| NewsClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| NewsClassName | string | 否 | 分类名称 |
| NewsTitle | string | 是 | 标题 |
| NewsContent | string | 是 | 内容 |
| NewsStatus | int | 是 | 状态：0新增，10发布，11撤下 |
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
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| PointsValueList | array object | 否 | 积分赠送配置值列表（接口） |
| StudyPersonList | array object | 否 | 人员足迹列表 |
| ModuleRelationList | array object | 否 | 关联模块列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BrowseCount | int | 否 | 浏览人数 |
| ViewCount | int | 否 | 浏览人次（同一人可累积） |
| UploadCount | int | 否 | 上传人数 |
| ReportCount | int | 否 | 汇报人数 |
| MyBrowseStatus | int | 否 | 当前浏览人的查看状态：0未阅，1已阅 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddNews | 操作 | 是 | 新增 |
| EditNews | 操作 | 是 | 修改 |
| DeleteNews | 操作 | 是 | 删除 |
| PublishNews | 操作 | 是 | 发布 |
| RemoveNews | 操作 | 是 | 撤下 |
| GetNewsFieldListByPage | 查询 | 是 | 根据页面，获取可选字段列表 |
| GetNewsList | 搜索 | 是 | 搜索列表 |
| GetNewsBySysNo | 查询 | 是 | 根据编码，获取详情 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| NewsType | int | 是 | 类型（枚举） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowPointsValueList | int | 否 | 是否显示积分配置列表 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况（MyBrowseStatus的开关） |
| IsShowModuleRelationList | int | 否 | 是否显示关联模块列表 |

#### NewsPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsPersonSysNo | int | 是 | 人员足迹系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| NewsPersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：3浏览 |
| BrowseCount | int | 是 | 浏览次数 |
| Remark | string | 否 | 备注 |

#### ModuleRelationList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 700101 | 新闻模块 | 党建动态 |  | 新增页 |
| 700102 |  | 党建动态 |  | 修改页 |
| 700103 |  | 党建动态 |  | 详情页 |
| 700104 |  | 党建动态 |  | 列表页 |
| 700201 |  | 红线之外 |  | 新增页 |
| 700202 |  | 红线之外 |  | 修改页 |
| 700203 |  | 红线之外 |  | 详情页 |
| 700204 |  | 红线之外 |  | 列表页 |



