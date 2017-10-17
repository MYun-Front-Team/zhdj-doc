# 获取好友申请列表（其他人加我） {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取好友申请列表

_**【应用场景】**_

获取好友申请列表

注：以UserSysNo换取Person，然后获取我的好友申请列表。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etFriendJoinList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 搜索条件 |
| Limit | object | 否 | 限制条件 |

> #### Sorts说明 \(数组\) {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsDescending | int | 是 | 是否倒序：0否，1是 |
| Name | string | 是 | 排序字段名称：如时间CreateTime，其它见模块说明 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FriendJoinSysNo | int | 是 | 好友申请编码 |
| Person | object | 是 | 成员实体（见基础模块登录） |
| JoinStatus | int | 是 | 加入状态：0申请中，1加入，2拒绝 |
| JoinReason | string | 否 | 申请理由 |
| RefuseReason | string | 否 | 拒绝理由 |



