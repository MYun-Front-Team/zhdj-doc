# 获取班级日课程列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取班级日课程列表

_**【应用场景】**_

获取班级日课程列表

_**【接口地址】**_

[http://ip:port/EduQuery/Class/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ClassDayCourseList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 班级系统编码 |
| DayWeek | int | 是 | 星期（如周一） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSysNo | int | 是 | 课程系统编码 |
| CourseName | Nvarchar（50） | 是 | 课程名称 |



