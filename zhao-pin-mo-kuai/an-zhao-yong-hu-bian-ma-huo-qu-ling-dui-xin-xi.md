# 按照用户编码获取领队信息
##### _【功能说明】_ {#【功能说明】}

按照用户编码获取领队信息

_**【应用场景】**_

按照用户编码获取领队信息


_**【接口地址】**_

http://ip:port/RecruitQuery/Leader/GetLeaderByPersonSysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 |人员编码|


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaderSysNo| int| 是 |领队编码|
| ActiveStatus| int| 是 |激活状态(0待绑定 ，10已激活，11已禁用) |
| CellPhoneNo| string | 是 |手机 |
| IDCard| string | 是 |身份证|
| RealName| string | 是 |姓名|
| PersonIDCardPathList | array string |是 | 身份证图片列表 |
| PersonIDCardUrlList | array string | 是 | 身份证图片列表 |
| PersonIDCardPathOtherList | array string | 否 | 身份证图片反面列表 |
| PersonIDCardUrlOtherList | array string | 否 | 身份证图片反面列表 |
| PersonSysNo| int| 是 |人员编码|
| LastLoginDate| string | 是 |最后登录时间 |














