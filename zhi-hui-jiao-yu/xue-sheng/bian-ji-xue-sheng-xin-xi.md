# 编辑学生信息

##### _【功能说明】_ {#【功能说明】}

编辑学生信息

_**【应用场景】**_

编辑学生信息

_**【接口地址】**_

http://ip:port/EduAction/Student/EditStudent

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentSysNo | int | 是 |学生系统编码 |
| ClassSysNo | int | 否 | 学生班级编码 |
| StudentNo| string| 否 | 学号 |
| UnionNo| string|否 | 学籍号 |
| ClassStudentType| int | 否| 类型： 1班长，2副班长，99学生|






> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignSysNo| int| 是 | 打卡编码 |
| StudentBase | object | 是 | 基础字段 |
| StudentStatistic | object | 否 | 统计字段 |













