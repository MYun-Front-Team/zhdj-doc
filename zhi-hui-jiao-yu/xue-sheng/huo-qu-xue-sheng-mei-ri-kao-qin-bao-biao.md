# 获取学生每日考勤报表

##### _【功能说明】_ {#【功能说明】}

获取学生每日考勤报表

_**【应用场景】**_

获取学生每日考勤报表

_**【接口地址】**_

http://ip:port/EduQuery/Student/GetSignReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Date| datetime| 是 | 日期 |
| DataRangeSysNo| int| 是 | 班级|




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Items| array[item]| 是 | 明细 |
| Total| object | 否 | 汇总 |

### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName| string| 是 | 姓名 |
| IsSign|int| 是 |当日是否签到 |

### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalCount| int| 是 |总人数 |
| SignCount| int| 是 | 已签到|
| NoSignCount| int| 是 | 未签到|




