# 获取选课学生列表
##### _【功能说明】_ {#【功能说明】}

获取选课学生列表


_**【应用场景】**_
获取选课学生列表


_**【接口地址】**_

http://ip:port/EduQuery/CourseSelect/GetCourseSelectItemStudentList


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectItemSysNo| int| 是 | 选课课程系统编码|
| StudentStatusList|array int| 是 | 状态（0圈中，10已选,11撤销）|
| IsCheatList|array  int| 是 |是否预留生|






> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectItemStudentSysNo| int| 是 | 系统编码|
| StudentSysNo| int| 是 |学生编码 |
| PersonSysNo| int| 是 | 学生人员编码|
| StudentStatus| int| 是 | 状态（0圈中，10已选）|
| IsCheat| int| 是 |是否预留生|
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| PersonName| string| 是 | 学生名称|
| InUser| string| 是 | 操作人|
| CreateTime| string| 是 |操作时间|






