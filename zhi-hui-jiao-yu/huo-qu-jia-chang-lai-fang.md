# 获取家长来访

##### _【功能说明】_ {#【功能说明】}

获取家长来访

_**【应用场景】**_

获取家长来访

_**【接口地址】**_

http://ip:port/EduQuery/Student/GetParentComing


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 是 | 家长人员编码 |
| StudentSysNo| int | 是 | 学生编码|
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| StartDate| datetime| 否 | 开始时间|
| EndDate| datetime| 否 | 结束时间 |
| ParentRealName| string| 是 | 家长姓名 |
| ParentPersonCellPhoneNo| string| 是 | 家长手机 |
| StudentRealName| int | 是 | 学生姓名|


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParentComingSysNo| int| 是 | 来访编码 |
| Student | StudentBase | 是 | 学生 |
| ParentPerson| Person| 是 | 家长 |
| PersonSysNo| int | 是 | 家长人员编码 |
| StudentSysNo| int | 是 | 学生编码|
| StudentPersonSysNo| int | 是 | 学生人员编码|


