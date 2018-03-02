# 设置个人通讯录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置个人通讯录

_**【应用场景】**_

设置个人通讯录

注：通过UserSysNo获取PersonSysNo，作为通讯录的所有者；

通过手机号获取好友的PersonSysNo（可为0）；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMailList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员系统编码 |
| FriendType | int | 是 | 通讯录类型：0手机通讯录 |
| FriendMailList | array string | 是 | 通讯录列表 |

#### FriendMail {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FriendCellPhoneNo | string | 是 | 手机号 |
| FriendPersonName | string | 是 | 备注姓名 |
| FriendCompanyName | string | 否 | 备注公司 |



