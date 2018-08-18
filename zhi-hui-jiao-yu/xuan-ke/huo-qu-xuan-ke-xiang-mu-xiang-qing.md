# 获取选课课程列表
##### _【功能说明】_ {#【功能说明】}

获取选课课程列表


_**【应用场景】**_
获取选课课程列表


_**【接口地址】**_

http://ip:port/EduQuery/CourseSelect/GetCourseSelectItemList


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectSysNo| int| 是 | 选课系统编码|
| ItemTypeList|array int| 是 | 课程类型（1长课时，2短课时上，3短课时下，4通用课时） |
| Limit| CourseSelectItemLimit| 是 | 显示限制|
| PickPersonSysNo| int| 是 | 选课人系统编码|
| StudentStatusList|array int| 是 |显示当前学课学生状态0圈中，10已报名，11撤销（和PickPersonSysNo一起传才有效） |





> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectItemSysNo| int| 是 | 选课课程系统编码|
| ItemType| int| 是 | 课程类型（1长课时，2短课时上，3短课时下，4通用课时） |
| CourseStart| datetime| 是 |课程开始 |
| CourseEnd| string| 是 | 课程结束 |
| CourseSysNo| int| 否 |课程主键 |
| CourseName | Nvarchar\(50\) | 否  | 课程名|
| TeacherName| string| 是 | 任课老师|
| IsFree| int| 是 | 是否免费 |
| Price| Decimal| 否 | 费用|
| LimitCount| int| 是 | 最多报名人数 |
| PickCount| int| 是 | 已报名人数 |
| CheatCount| int| 是 | 预留生人数 |
| IsNeedPickStudent| int| 否 | 是否限定报名范围|
| CourseSelectItemDayList | array CourseSelectItemDay| 是 | 上课时间 |
| StudentStatus| int| 是 |显示当前学课学生状态0圈中，10已报名，11撤销 |
| CourseRemark| string| 是 | 课程备注|





####CourseSelectItemDay

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WeekDay| int| 是 | (0周日，1周一，2周二，3周三，4周四，5周五，6周六) |
| StartTime| datetime| 是 |上课时间 |
| EndTime| datetime| 是 | 下课时间 |

#### Limit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowCourseSelectItemDayList  | int | 是 | 是否展示上课时间|






