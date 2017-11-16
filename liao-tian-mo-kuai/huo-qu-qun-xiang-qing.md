# 创建群 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

创建群

_**【应用场景】**_

创建群

注：群类型=11002会话 表示的是单聊群。

注：创建人即是第一个群成员+创建人权限+管理员权限。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)GetGroupBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupBase | object | 是 | 基础字段 |
| GroupStatistic | object | 否 | 计算字段 |



