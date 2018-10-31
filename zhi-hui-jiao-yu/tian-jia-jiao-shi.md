# 添加教师

##### _【功能说明】_ {#【功能说明】}

添加教师

_**【应用场景】**_

添加教师

_**【接口地址】**_

http://ip:port/EduAction/Teacher/AddTeacher

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNoList |array[int] | 否 | 负责班级 |
| CellPhoneNo| string| 是 | 手机号 |
| LoginPwd| string | 是 | 密码|
| RealName| string | 是 | 姓名|
| RoleSysNoList| array[int]| 是 | 角色编码 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 是 | 教师编码 |



