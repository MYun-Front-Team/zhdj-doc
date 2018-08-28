# 添加选课课程详情
##### _【功能说明】_ {#【功能说明】}

添加选课课程详情

_**【应用场景】**_

添加选课课程详情

_**【接口地址】**_

http://ip:port/EduAction/CourseSelect/AddCourseSelectItem



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectSysNo| int| 否 | 选课系统编码|
| ItemType| int| 是 | 课程类型（1长课时，2短课时上，3短课时下，4通用课时） |
| CourseStart| datetime| 是 |课程开始 |
| CourseEnd| string| 是 | 课程结束 |
| CourseSysNo| int| 否 |课程主键（可以为0，如果为0，则需要传课程名，课程描述） |
| CourseName | Nvarchar\(50\) | 否 | 课程名|
| CourseContent | string | 否 | 课程描述 |
| FilePathList | array string | 否 | 课程附件路径列表 |
| TeacherName| string| 是 | 任课老师|
| IsFree| int| 是 | 是否免费 |
| Price| Decimal| 否 | 费用|
| LimitCount| int| 是 | 最多报名人数 |
| IsNeedPickStudent| int| 否 | 是否限定报名范围|
| PickRuleTemplateList | array object | 是 | 选人规则 |
| CourseSelectItemDayList | array CourseSelectItemDayAdd| 是 | 上课时间 |







