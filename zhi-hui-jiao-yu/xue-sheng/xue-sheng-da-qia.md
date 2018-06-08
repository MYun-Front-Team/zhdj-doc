# 学生打卡

##### _【功能说明】_ {#【功能说明】}

学生打卡

_**【应用场景】**_

学生打卡

_**【接口地址】**_

http://ip:port/EduAction/Student/StudentSign

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo| string| 是 | 卡号 |
| FilePathList|array string| 是 | 图片|



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentBase | object | 是 | 基础字段 |
| StudentStatistic | object | 否 | 统计字段 |













