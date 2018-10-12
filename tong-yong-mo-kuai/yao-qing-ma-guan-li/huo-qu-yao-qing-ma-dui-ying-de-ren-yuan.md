# 获取邀请码对应的人员

##### _【功能说明】_ {#【功能说明】}

获取邀请码对应的人员

_**【应用场景】**_

获取邀请码对应的人员

_**【接口地址】**_

http://ip:port/BasicQuery/InvitationCode/GetInvitationPeron

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InvitationCode| string| 否 | 邀请码|


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 否 |邀请的人编码 |
| PersonName| string| 否 |邀请人员名称 |
| FileUrlList | array string | 否 | 头像图片列表 |






