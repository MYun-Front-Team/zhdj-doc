# 设置群管理员 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置群管理员

_**【应用场景】**_

设置群管理员

注：根据IsManager的状态来区分是设置为管理员还是移除管理员。

注：需判断操作人是否拥有设置的权限（管理员\创建人），管理员不能移除创建人的权限。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupManager

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| PersonSysNo | int | 是 | 群成员系统编码 |
| IsManager | int | 是 | 是否管理员：0否，1是 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



