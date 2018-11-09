# 获取学生/教师打卡记录

##### _【功能说明】_ {#【功能说明】}

获取学生/教师打卡记录

_**【应用场景】**_

获取学生/教师列表

_**【接口地址】**_

http://ip:port/EduQuery/Student/GetStudentSignList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsAgent | int | 否 | 是否显示自己代理人的消息 |
| StudentSysNo| int | 否 | 学生编码 |
| StartSignTime| datetime| 否 | 开始时间|
| EndSignTime| int | 否 | 结束时间 |
| CardNo| string| 是 | 卡号 |
| SignTypeList| int| 否 | 0进校/1出校 |
| DataRangeSysNoList | int | 是 | 学生数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| TeacherDataRangeSysNoList | int | 是 | 教师数据范围树枝叶编码列表 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignSysNo| int| 是 | 打卡编码 |
| PersonSysNo| int| 是 | 人员编码 |
| StudentSysNo| int| 是 | 学生编码 |
| TeacherSysNo| int| 是 | 教师编码 |
| FilePathList|array string| 否 | 图片|
| FileUrlList|array string| 否 | 图片|
| CreateTime| datetime| 是 | 时间 |
| PersonName| string| 是 | 人员名称|
| SignType| int| 否 | 0进校/1出校 |
| SignTime| datetime| 否| 打卡时间 |
| CardNo| string| 是 | 卡号 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |




