# 聊天模块-字段说明 {#新增河流}

> #### GroupBase基础字段 {#请求数据}

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
| FileUrlList | array string | 否 | 文件url列表 |

> #### GroupStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalFriendCount | int | 否 | 我的好友总数 |
| GroupPersonCount | int | 否 | 某个群的成员数量 |
| FriendInGroupCount | int | 否 | 某个群的我的好友数量 |
| JoinGroupCount | int | 否 | 我的加群数量 |
| GroupJoinStatus | int | 否 | 某个群我的加入状态：0申请中，1加入，2拒绝 |
| IsFriend | int | 否 | 是否朋友：0否，1是 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserGender | int | 否 | 性别：0全部，1男，2女 |
| KeyWord | string | 否 | 关键字搜索 |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileUrlList | int | 否 | 是否显示文件图片列表 |
| IsShowTotalFriendCount | int | 否 | 是否显示我的好友总数 |
| IsShowGroupPersonCount | int | 否 | 是否显示某个群的成员数量 |
| IsShowFriendInGroupCount | int | 否 | 是否显示某个群的我的好友数量 |
| IsShowJoinGroupCount | int | 否 | 是否显示我的加群数量 |
| IsShowGroupJoinStatus | int | 否 | 是否显示我的加群状态 |
| IsShowAuditPerson | int | 否 | 是否显示我的加群审核人 |
| IsShowIsFriend | int | 否 | 是否显示是否朋友 |

####  {#应答数据-（巡河记录数组）}

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |




