# 设置账户在线状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置账户在线状态

_**【应用场景】**_

设置账户在线状态

注：如果“登录授权Token”不为空，则跟账户表的“LastLoginToken”的值比对，相同返回1，否则0；

_**【接口地址】**_

[http://ip:port/ChatAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Chat](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etOnlineStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OnlineStatus | int | 是 | 在线状态：0离线，1在线 |
| OnlineStatusForDisplay | int | 否 | 是否打开APP：0否，1是 |
| AccessToken | string | 否 | 登录授权Token |

#### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AccessStatus | int | 是 | 授权状态：0失效，1正常 |



