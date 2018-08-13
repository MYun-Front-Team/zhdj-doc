# 获取选课列表

##### _【功能说明】_ {#【功能说明】}

获取选课列表


_**【应用场景】**_

获取选课列表


_**【接口地址】**_

http://ip:port/EduQuery/CourseSelect/GetCourseSelectList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord| string| 是 | 关键字|
| CourseSelectStatusList|array int| 是 | 选课状态（0草稿，10已发布）|
| DateStatusList|array int| 是 | 进行状态（0未开始，10进行中，11已过期）|




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSelectSysNo| int| 是 | 选课系统编码|
| CourseSelectName| string| 是 | 选课名称|
| SelectStart| datetime| 是 | 报名开始|
| SelectEnd| datetime| 是 | 报名结束|
| CourseSelectStatus| int| 是 | 选课状态（0草稿，10已发布）|
| DateStatus| int| 是 | 进行状态（0未开始，10进行中，11已过期）|
| InUser| string| 是 | 创建人|







