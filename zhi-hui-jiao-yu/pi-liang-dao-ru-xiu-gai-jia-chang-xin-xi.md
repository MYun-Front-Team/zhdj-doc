# 批量导入修改家长信息

##### _【功能说明】_ {#【功能说明】}

批量导入修改家长信息

_**【应用场景】**_

批量导入修改家长信息

_**【接口地址】**_

http://ip:port/EduAction/Student/ImportStudentParent

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParentImports| array[ParentImport]| 是 |导入元素 |

#### ParentImport

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentSysNo| int | 是 |学生系统编码 |
| ParentSysNo1| int | 否 | 家长1系统编码 |
| ParentName1| string| 否 | 家长1姓名 |
| ParentPhoneNo1| string| 否 | 家长1手机号  |
| ParentPhoneNoNew1| string| 否 | 家长1新手机号 |
| ParentSysNo2| int | 否 | 家长2系统编码 |
| ParentName2| string| 否 | 家长2姓名 |
| ParentPhoneNo3| string| 否 | 家长2手机号  |
| ParentPhoneNoNew2| string| 否 | 家长2新手机号 |
| ParentSysNo3| int | 否 | 家长3系统编码 |
| ParentName3| string| 否 | 家长3姓名 |
| ParentPhoneNo3| string| 否 | 家长3手机号  |
| ParentPhoneNoNew3| string| 否 | 家长3新手机号 |
| ParentSysNo4| int | 否 | 家长4系统编码 |
| ParentName4| string| 否 | 家长4姓名 |
| ParentPhoneNo4| string| 否 | 家长4手机号  |
| ParentPhoneNoNew4| string| 否 | 家长4新手机号 |
| ParentSysNo5| int | 否 | 家长5系统编码 |
| ParentName5| string| 否 | 家长5姓名 |
| ParentPhoneNo5| string| 否 | 家长5手机号  |
| ParentPhoneNoNew5| string| 否 | 家长5新手机号 |
| ParentSysNo6| int | 否 | 家长6系统编码 |
| ParentName6| string| 否 | 家长6姓名 |
| ParentPhoneNo6| string| 否 | 家长6手机号  |
| ParentPhoneNoNew6| string| 否 | 家长6新手机号 |




> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  | int | 是 |家长编码 |















