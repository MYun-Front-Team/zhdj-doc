# 获取党员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员列表

_**【应用场景】**_

获取党员列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetPartyMember](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)List

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  | 是 | 搜索条件 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberBase | PartyMemberBase | 是 | 基本字段 |
| PartyMemberStatistic | PartyMemberStatistic | 是 | 统计计算字段 |
| ActivityInfoList | array\[ActivityInfo\] | 是 | 活动汇总计算字段 |
| StudyInfoList | array\[StudyInfo\] | 是 | 学习汇总计算字段 |
| ~~Person~~ | ~~object~~ | ~~是~~ | ~~Person实体（见登录接口）~~ |



