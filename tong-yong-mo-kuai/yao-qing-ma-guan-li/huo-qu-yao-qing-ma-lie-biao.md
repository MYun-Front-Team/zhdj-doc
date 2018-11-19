# 获取邀请码列表

##### _【功能说明】_ {#【功能说明】}

获取邀请码列表

_**【应用场景】**_

获取邀请码列表

_**【接口地址】**_

http://ip:port/BasicQuery/InvitationCode/GetInvitationCodeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsUsedList|array[int] | 否 | 1已用 0未用|
| PersonSysNo| int | 否 |人员编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InvitationCode| string| 否 | 邀请码|
| IsUsed| int | 否 |是否使用 |
| PersonToSysNo| int | 否 |邀请的人 |
| PersonName| string| 否 |邀请人员名称 |
| FileUrlList | array string | 否 | 头像图片列表 |
| UsedDate| datetime| 否 |使用时间 |





