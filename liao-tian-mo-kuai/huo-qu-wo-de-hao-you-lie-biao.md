# 获取我的好友列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取我的好友列表

_**【应用场景】**_

获取我的好友列表

注：以UserSysNo换取Person，然后获取我的好友列表。

注：首字母优先级：好友备注名首字母&gt;昵称首字母&gt;真实姓名首字母

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMyFriendList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FirstLetter | string | 否 | 首字母 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 成员实体（见基础模块登录） |
| FriendPersonName | string | 否 | 备注好友姓名 |



