# 获取考勤统计

##### _【功能说明】_ {#【功能说明】}

获取考勤统计


_**【应用场景】**_

获取考勤统计


_**【接口地址】**_

http://ip:port/EduQuery/Report/GetPersonLine

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentTotal| int | 是 | 学生总数|
| StudentIn|int| 是 | 学生在校|
| StudentOut|int| 是 | 学生离校|
| TeacherTotal|int| 是 | 教师总数|
| TeacherIn|int| 是 | 教师在校|
| TeacherOut|int| 是 | 教师离校|













