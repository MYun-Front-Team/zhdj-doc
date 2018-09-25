# 学生打卡

##### _【功能说明】_ {#【功能说明】}

学生打卡

_**【应用场景】**_

学生打卡

_**【接口地址】**_

http://ip:port/EduAction/Student/GroupStudentSign

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardInfos|array[CardInfo]| 否 | 卡信息|


 #### CardInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo| string| 是 | 卡号 |
| SignTime| datetime| 否| 打卡时间 |
| SignType| int| 否 | 1进校/ 2出校 |

















