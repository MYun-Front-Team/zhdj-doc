# 获取群成员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取群成员列表

_**【应用场景】**_

获取群成员列表

注：Limit可控制IsFriend、AuditPerson的值。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupPersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| IsFriend | int | 否 | 是否朋友 |
| IsManager | int | 否 | 是否管理员 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 成员实体（见基础模块登录） |
| IsFounder | int | 是 | 是否创建人 |
| IsManager | int | 是 | 是否管理员 |
| AuditPerson | object | 否 | 加入审核人成员实体 |
| GroupStatistic | object | 否 | 计算字段（见模块说明） |



