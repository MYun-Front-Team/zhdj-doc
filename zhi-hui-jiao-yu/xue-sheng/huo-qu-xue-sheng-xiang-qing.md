# 获取学生详情

##### _【功能说明】_ {#【功能说明】}

获取学生详情

_**【应用场景】**_

获取学生详情

_**【接口地址】**_

http://ip:port/EduQuery/Student/GetStudentBySysNo


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentSysNo | int| 是 | 学生编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentBase | object | 是 | 基础字段 |
| StudentStatistic | object | 否 | 统计字段 |





