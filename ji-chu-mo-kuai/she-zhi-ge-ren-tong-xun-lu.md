# 设置个人通讯录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置个人通讯录

_**【应用场景】**_

设置个人通讯录

注：通过UserSysNo找到自己的PersonSysNo; 

通过FriendCellPhoneNo找到朋友的PersonSysNo，不存在则为0；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMailList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FriendType | int | 是 | 通讯录类型：0手机通讯录 |
| FriendCellPhoneNo | string | 是 | 手机号 |
| FriendPersonName | string | 是 | 备注姓名 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |



