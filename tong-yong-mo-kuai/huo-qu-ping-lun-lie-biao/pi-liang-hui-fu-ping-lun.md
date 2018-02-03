# 批量回复评论 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

批量回复评论

_**【应用场景】**_

批量回复评论

注：回复内容记录通用-审核，审核人即操作人；

_**【接口地址】**_

[http://ip:port/UMAction/Comment/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etCommentReply

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentReplyList | array object | 是 | 评论回复列表 |

> CommentReply说明

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentSysNo | int | 是 | 评论系统编码 |
| ShowStatus | int | 否 | 显示状态：0不显示，1显示 |
| DeleteStatus | int | 否 | 删除状态：0否，1是 |
| SortNo | int | 否 | 置顶排序 |
| ReplyContent | string | 是 | 回复内容 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



