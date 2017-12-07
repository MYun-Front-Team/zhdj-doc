# 设置评论状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置评论状态

_**【应用场景】**_

设置评论状态

注：“显示状态”只影响前台展现的屏蔽，“删除状态”则物理删除该评论；

_**【接口地址】**_

[http://ip:port/UMAction/Comment/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etCommentStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentSysNo | int | 是 | 评论系统编码 |
| ShowStatus | int | 否 | 显示状态：0不显示，1显示 |
| DeleteStatus | int | 否 | 删除状态：0否，1是 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



