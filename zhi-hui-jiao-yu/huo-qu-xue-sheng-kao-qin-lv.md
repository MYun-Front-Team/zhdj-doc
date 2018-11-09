# 获取学生考勤率

##### _【功能说明】_ {#【功能说明】}

获取学生考勤率


_**【应用场景】**_

获取学生考勤率


_**【接口地址】**_

http://ip:port/EduQuery/Report/GetStudentAttendance

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| Date| datetime| 是 | 时间 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentTotal| int | 是 | 学生总数|
| StudentIn|int| 是 | 正常签到|
| StudentOut|int| 是 | 正常签退|














