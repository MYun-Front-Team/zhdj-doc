# 获取选课详情

##### _【功能说明】_ {#【功能说明】}

获取选课详情


_**【应用场景】**_

获取选课详情


_**【接口地址】**_

http://ip:port/EduQuery/CourseSelect/GetCourseSelectBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectSysNo| int| 是 | 选课系统编码|




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectSysNo| int| 是 | 选课系统编码|
| CourseSelectName| string| 是 | 选课名称|
| SelectStart| datetime| 是 | 报名开始|
| SelectEnd| datetime| 是 | 报名结束|
| CourseSelectStatus| int| 是 | 选课状态（0草稿，10已发布）|
| IsOverdue| int| 是 | 是否过期（0正常，1过期）|
| InUser| string| 是 | 创建人|



