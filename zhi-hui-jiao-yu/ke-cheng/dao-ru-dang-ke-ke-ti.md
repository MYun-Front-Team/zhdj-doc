# 导入党课课题


_**【接口地址】**_

http://ip:port/EduAction/Course/ImportPartyCourse

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataList | array object | 是 | 课题列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeacherName | string | 是 | 教员姓名 |
| CellPhoneNo | string | 是 | 教员电话 |
| CourseName | string | 是 | 课程名称 |
| CourseClassName | string | 是 | 课题类别 |
| CourseContent | string | 是 | 课程内容 |
| CourseStatus | int | 是 | 0保存，1提交审批, 10审核通过 |
| Post | string | 是 | 教员职务 |
| ApplicableObject | string | 是 | 适用对象 |
| DepartmentName | string | 否 | 所在单位 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



