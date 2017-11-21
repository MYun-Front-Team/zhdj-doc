# 朋友圈模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MomentsSysNo | int | 是 | 系统编码 |
| MomentsType | int | 否 | 类型（枚举） |
| MomentsClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| MomentsTitle | string | 否 | 标题 |
| MomentsContent | string | 是 | 内容 |
| PublishPersonSysNo | int | 否 | 发布人员编码 |
| PublishTime | string | 否 | 发布时间 |
| PersonPost | string | 否 | 岗位（业务模块冗余） |
| PersonDepartment | string | 否 | 部门（业务模块冗余） |
| PublishPerson | object | 否 | 发布人员实体对象 |
| Remark | string | 否 | 备注 |
| SortNo | int | 否 | 排序 |
| IsDisplay | int | 否 | 是否隐藏：0否，1是 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |
| MomentsPersonList | array object | 否 | 人员足迹列表 |
| ModuleRelationList | array object | 否 | 关联模块列表（见活动） |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignGoodCount | int | 否 | 点赞人数 |
| SignReplyCount | int | 否 | 回复人数 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddMoments | 操作 | 是 | 新增 |
| SetMomentsGood | 操作 | 是 | 点赞 |
| SetMomentsReply | 操作 | 是 | 回复 |
| SetMomentsReaded | 操作 | 是 | 设置已读 |
| SetMomentsDisplay | 操作 | 是 | 隐藏 |
| GetMomentsList | 搜索 | 是 | 搜索列表 |
| GetMomentsBySysNo | 查询 | 是 | 根据编码，获取详情 |
| GetUnReadedCount | 查询 | 是 | 获取未读数量 |
| GetUnReadedList | 查询 | 是 | 获取未读列表 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索 |
| PublishStartTime | string | 否 | 发布开始时间 |
| PublishEndTime | string | 否 | 发布结束时间 |
| IsDisplay | int | 否 | 是否隐藏：0否，1是（不传查全部） |
| IsOwner | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowPersonList | int | 否 | 是否显示人员列表 |
| IsShowModuleRelationList | int | 否 | 是否显示关联模块列表 |
| IsShowPositionList | int | 否 | 是否显示定位列表（该值必须在IsShowPersonList=1时有效，返回结果按正序排列，参数值1则为返回一条） |

#### MonentsPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MonentsPersonSysNo | int | 是 | 人员足迹系统编码 |
| FromPerson | object | 是 | 发表人员实体 |
| ToPerson | object | 是 | 接收人员实体 |
| IsReaded | int | 是 | 是否已读：0否，1是 |
| PersonStatus | int | 是 | 状态：0发布定位，1浏览，2点赞，3转发，4分享 ，5回复 |
| SignCount | int | 是 | 足迹次数 |
| SignTime | string | 是 | 最近足迹时间 |
| SignPlace | string | 否 | 最近足迹地点（定位） |
| SignContent | string | 否 | 足迹内容（回复） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Remark | string | 否 | 备注 |
| Moments | object | 否 | 朋友圈记录实体对象（只有在获取未读列表中返回） |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |




