#设置临时课表

##### _【功能说明】_ {#【功能说明】}

设置临时课表

_**【应用场景】**_

设置临时课表

_**【接口地址】**_

http://ip:port/EduAction/Class/SetClassDayCourseTemp

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassDayCourses| array[ClassDayCourse]| 是 | 课程|
| StartDate| datetime| 是 | 开始时间|
| EndDate| datetime| 是 | 结束时间|



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassDayCourseSysNo| int | 是 | 课表系统编码 |
| CourseSysNo | int | 是 | 课程系统编码 |






