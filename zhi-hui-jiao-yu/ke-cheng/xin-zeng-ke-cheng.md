# 新增课程 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增课程

_**【应用场景】**_

新增课程

_**【接口地址】**_

[http://ip:port/EduAction/Course/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddCourse

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| CourseClassSysNo | int | 否 | 分类编码（通用） |
| CourseName | Nvarchar\(50\) | 是 | 课程名称 |
| CourseContent | string | 否 | 课程描述 |
| CourseStatus | int | 是 | 课程状态：0新增，10上架，11下架 |
| TeacherSysNo | int | 否 | 教师系统编码 |
| TagSysNoList | array int | 否 | 适用对象标签编码列表 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 附件路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSysNo | int | 是 | 课程系统编码 |



