# 党课编辑课题


_**【接口地址】**_

http://ip:port/EduAction/Course/EditPartyCourse

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSysNo | int | 是 | 课题id |
| CourseClassSysNo | int | 是 | 分类编码（通用） |
| CourseName | string | 是 | 课程名称 |
| CourseContent | string | 是 | 课程描述 |
| CourseStatus | int | 是 | 0保存，1提交审批 |
| MemberSysNo | int | 是 | 党员系统编码 |
| ApplicableObject | string | 是 | 适用对象 |
| DepartmentSysNo | string | 是 | 所属单位 |
| FilePathList | array string | 否 | 附件列表 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




