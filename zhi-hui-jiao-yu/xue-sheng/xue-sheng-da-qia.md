# 学生打卡

##### _【功能说明】_ {#【功能说明】}

学生打卡

_**【应用场景】**_

学生打卡

_**【接口地址】**_

http://ip:port/EduAction/Student/StudentSign

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo| string| 是 | 卡号 |
| FilePathList|array string| 否 | 图片|
| SignTime| datetime| 否| 打卡时间 |
| SignType| int| 否 | 进校/出校 |
| PersonSysNo| int| 否 | 学生编码 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignSysNo| int| 是 | 打卡编码 |
| StudentBase | object | 是 | 基础字段 |
| StudentStatistic | object | 否 | 统计字段 |
| PersonName| string| 是 | 人员名字 |
| CardType| int| 是 | 卡类型：3学生考勤卡，4学生一卡通，5教师考勤卡|
| ClassName| string| 是 | 班级名称 |
| SchoolName| string| 是 | 学校名称 |

