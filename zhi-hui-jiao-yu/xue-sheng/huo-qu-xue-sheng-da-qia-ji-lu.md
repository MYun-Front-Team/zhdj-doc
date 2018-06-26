# 获取学生打卡记录

##### _【功能说明】_ {#【功能说明】}

获取学生打卡记录

_**【应用场景】**_

获取学生列表

_**【接口地址】**_

http://ip:port/EduQuery/Student/GetStudentSignList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsAgent | int | 否 | 是否显示自己代理人的消息 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignSysNo| int| 是 | 打卡编码 |
| PersonSysNo| int| 是 | 人员编码 |
| StudentSysNo| int| 是 | 人员编码 |
| FilePathList|array string| 否 | 图片|
| FileUrlList|array string| 否 | 图片|
| CreateTime| datetime| 是 | 时间 |














