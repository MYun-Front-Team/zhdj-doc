# 获取学期列表

##### _【功能说明】_ {#【功能说明】}

获取学期列表


_**【应用场景】**_

获取学期列表


_**【接口地址】**_

http://ip:port/EduQuery/Student/GetSemesterList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 学校数据范围树枝叶编码 |




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SemesterSysNo| int| 是 | 系统编码|
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| SemesterName| string| 是 |学期名称 |
| SemesterCode| string| 是 |学期编码 |

