# 添加学生信息

##### _【功能说明】_ {#【功能说明】}

添加学生信息

_**【应用场景】**_

添加学生信息

_**【接口地址】**_

http://ip:port/EduAction/Student/AddStudent

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 学生班级编码 |
| StudentNo| string| 否 | 学号 |
| UnionNo| string|否 | 学籍号 |
| ClassStudentType| int | 否| 类型： 1班长，2副班长，99学生|
| FreeType| int | 否 |1缴费用户、0未缴费用户、2公免用户 |
| PersonName | string | 是 | 昵称 |
| RealName | string | 是 | 真实姓名 |
| UserGender | int | 是  | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| IDCard | string | 否 | 身份证 |
| BloodType| string| 否 | 血型|
| Anaphylaxis| string| 否 |过敏史|
| Hobby| string| 否 |爱好|
| Remark| string| 否 |备注|
| IDCardType | int| 否 | 证件类型|

> #### 返回数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentSysNo | int | 是 | 学生编码 |
| PersonSysNo | int | 是 | 人员编码 |

