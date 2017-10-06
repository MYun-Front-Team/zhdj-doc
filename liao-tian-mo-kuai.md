# 聊天模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| GroupType | int | 是 | 群类型（枚举） |
| GroupClassSysNo | int | 否 | 群分类系统编码（会话类型时可为空）（类别树） |
| GroupID | string | 否 | 群ID |
| GroupName | string | 是 | 群名称 |
| GroupDesc | string | 否 | 群描述 |
| GroupAddress | string | 否 | 群地址 |
| PrivacyStatus | int |  | 隐私状态：0封闭（被搜索，不能看内容），1公开（被搜索，能看内容），2秘密（搜不到，不能看） |
| LifeCycleTime | string | 否 | 生命周期有效期 |
| IsNeedAudit | int | 否 | 是否需要审核（默认1需要审核） |
| Longitude | decimal\(18,10\) | 否 | 经度 |
| Latitude | decimal\(18,10\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 文件path路径列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonDataStatistics | object | 是 | 成员数据统计 |

> #### PersonDataStatistics说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalFriendCount | int | 是 | 好友总数 |
| FriendInGroupCount | int | 是 | 好友在某个群的数量 |
| GroupJoinCount | int | 是 | 加群数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddGroup | 操作 | 是 | 新增群 |
| EditGroup | 操作 | 是 | 修改群 |
| DeleteGroup | 操作 | 是 | 解散群 |
|  | 查询 | 是 |  |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserGender | int | 否 | 性别：0全部，1男，2女 |
| KeyWord | string | 否 | 关键字搜索 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |

####  {#应答数据-（巡河记录数组）}

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |




