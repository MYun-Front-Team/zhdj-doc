# 员工设置薪水、赏金

##### _【功能说明】_ {#【功能说明】}

员工设置薪水、赏金

_**【应用场景】**_
员工设置薪水、赏金


_**【接口地址】**_

http://ip:port/RecruitAction/Interview/EditInterviewPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewPersonSysNo| int | 是 | 面试人表编码 |
| Salary| Decimal| 否 | 面试人表编码 |
| WorkStartDay|datetime| 否 | 预计入职时间 |
| Reward|Decimal| 否 | 平台奖励 |
| EntryStatus|int | 否 | 入职状态（0待入职10已入职11未入职）|
| EntryDate|datetime| 否 | 入职时间 |
| EntryRemark|string| 否 | 入职备注 |








