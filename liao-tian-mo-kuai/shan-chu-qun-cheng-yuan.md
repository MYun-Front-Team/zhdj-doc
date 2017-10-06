# 删除群成员 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

删除群成员

_**【应用场景】**_

删除群成员

注：需判断操作人是否拥有设置的权限（管理员\创建人），管理员不能删除创建人。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/D](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)eleteGroupPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| PersonSysNo | int | 是 | 群成员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



