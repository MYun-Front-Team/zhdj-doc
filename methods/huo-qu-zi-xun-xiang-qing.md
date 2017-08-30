# 获取资讯记录详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取资讯记录详情

_**【应用场景】**_

获取资讯记录详情

_**【接口地址】**_

[http://ip:port/UMQuery/Info/GetInfoB](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)yInfoSysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否 | 资讯系统编码 |
| InfoLimit | array | 否 | 限制条件 |

> #### InfoLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowCover | int | 否 | 是否显示封面 |
| IsShowFileUrls | int | 否 | 是否显示文件图片列表 |
| IsShowFootPrintCount | int | 否 | 是否显示人员足迹总数 |
| IsShowFootPrintList | int | 否 | 是否显示人员足迹列表 |
| IsShowReplyCount | int | 否 | 是否显示回复总数 |
| IsShowReplyList | int | 否 | 是否显示回复列表 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |
| InfoTypeSysNo | int | 是 | 资讯类型编码 |
| InfoClassSysNo | int | 否 | 资讯分类编码 |
| InfoTitle | string | 是 | 资讯标题（主题） |
| InfoStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishUserSysNo | int | 否 | 发布人编码 |
| PublishUserName | string | 否 | 发布人 |
| PublishTime | string | 否 | 发布时间 |
| RemoveUserSysNo | int | 否 | 撤下人编码 |
| RemoveUserName | string | 否 | 撤下人 |
| RemoveTime | string | 否 | 撤下时间 |
| MaxPersonNum | int | 否 | 人数上限 |
| InfoPlace | string | 否 | 活动地点 |
| InfoSignUpStartTime | string | 否 | 报名开始时间 |
| InfoSignUpEndTime | string | 否 | 报名结束时间 |
| InfoStartTime | string | 否 | 活动开始时间 |
| InfoEndTime | string | 否 | 活动结束时间 |
| FileUrls | array string | 否 | 文件图片列表 |
| FootPrintCountList | array object | 否 | 人员足迹总数列表（见列表） |
| FootPrintList | array object | 否 | 人员足迹列表 |
| ReplyList | array object | 否 | 回复列表 |

#### FootPrintList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FootPrintSysNo | int | 是 | 人员足迹系统编码 |
| SourceType | int | 是 | 足迹类型：0客户，1用户，2部门 |
| SourceSysNo | int | 是 | 对应系统编码 |
| Name | string | 否 | 姓名 |
| CellPhoneNo | string | 否 | 手机 |
| FootPrintType | int | 否 | 足迹类型:0普通，1报名，2分享，3点赞 |
| PersonStatus | int | 是 | 状态：0报名/阅读/分享,1审核/确认，10签到/完成，11删除/请假 |
| IsEnable | int | 否 | 是否有效 |
| SignCount | int | 否 | 足迹数量 |
| SignTime | string | 否 | 足迹时间 |
| SignPlace | string | 否 | 足迹地点（签到/活动地） |
| SignJson | string | 否 | 端自定义字段（原样返回） |
| Reason | string | 否 | 原因 |
| Remark | string | 否 | 备注 |

#### ReplyList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReplySysNo | int | 是 | 回复系统编码 |
| SourceType | int | 是 | 足迹类型：0客户，1用户，2部门 |
| SourceSysNo | int | 是 | 对应系统编码 |
| ReplyTitle | string | 否 | 主题 |
| ReplyContent | string | 否 | 内容 |
| ReplyJson | string | 否 | 端自定义JSON |
| Remark | string | 否 | 备注 |



