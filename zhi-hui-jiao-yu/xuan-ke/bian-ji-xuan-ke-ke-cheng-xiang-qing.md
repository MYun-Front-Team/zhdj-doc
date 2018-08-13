# 编辑选课课程详情

##### _【功能说明】_ {#【功能说明】}

编辑选课课程详情

_**【应用场景】**_

编辑选课课程详情

_**【接口地址】**_

http://ip:port/EduAction/CourseSelect/EditCourseSelectItem



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectItemSysNo| int| 是 | 选课课程系统编码|
| TeacherName| string| 是 | 老师名称 |
| IsFree| int| 是 | 是否免费 |
| Price| Decimal| 否 | 费用|
| LimitCount| int| 是 | 最多报名人数（发布以后，只能改多，不能改少，发布前不限制） |







