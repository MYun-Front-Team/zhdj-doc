# 获取我的推荐好友列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取我的推荐好友列表

_**【应用场景】**_

获取我的推荐好友列表

注：由于手机通讯中的好友有些没有使用我们的系统，故Person实体中的PersonSysNo可能为0；

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMyRecommendFriendList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FriendType | int | 是 | 推荐类型：0手机通讯录 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 成员实体（见基础模块登录） |
| GroupStatistic | object | 否 | 计算字段（见模块说明） |



