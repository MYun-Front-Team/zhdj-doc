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
| FreeType| int | 是 |1缴费用户、0未缴费用户、2公免用户 |


























