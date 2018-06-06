# 修改课程 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改课程

_**【应用场景】**_

修改课程

_**【接口地址】**_

[http://ip:port/CourseAction/Course/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditCourse

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSysNo | int | 是 | 课程系统编码 |
| CourseName | Nvarchar\(50\) | 否 | 课程名称 |
| CourseContent | string | 否 | 课程描述 |
| CourseStatus | int | 否 | 课程状态：0新增，10上架，11下架 |
| TagSysNoList | array int | 否 | 适用对象标签编码列表 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 附件路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



