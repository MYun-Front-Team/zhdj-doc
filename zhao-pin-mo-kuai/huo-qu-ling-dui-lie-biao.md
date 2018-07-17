# 获取领队列表

##### _【功能说明】_ {#【功能说明】}

获取领队列表

_**【应用场景】**_

获取领队列表

_**【接口地址】**_
http://ip:port/RecruitQuery/Leader/GetLeaderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string | 否 |关键字|
| CellPhoneNo| string | 是 |手机 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CellPhoneNo| string | 是 |手机 |
| IDCard| string | 是 |身份证|
| RealName| string | 是 |姓名|
| PersonIDCardPathList | array string |是 | 身份证图片列表 |
| PersonIDCardUrlList | array string | 是 | 身份证图片列表 |
| PersonSysNo| int| 是 |人员编码|
| ActiveStatus| int| 是 |激活状态 |





