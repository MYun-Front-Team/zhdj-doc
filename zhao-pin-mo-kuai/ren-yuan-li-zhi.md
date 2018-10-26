# 人员离职
##### _【功能说明】_ {#【功能说明】}

人员离职


_**【应用场景】**_
人员离职


_**【接口地址】**_

http://ip:port/RecruitAction/Interview/QuitPersonToInterview

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewPersonSysNo| int | 是 | 面试人表编码 |
| QuitDate| datetime| 是 | 离职时间 |
| QuitType| int | 否 | 离职类型 |
| QuitReason| string| 是 | 离职原因  |
| QuitRemark| string| 否 | 离职备注 |
