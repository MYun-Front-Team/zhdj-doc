# 添加领队
##### _【功能说明】_ {#【功能说明】}

添加领队

_**【应用场景】**_

添加领队

手机号不能重复


_**【接口地址】**_

http://ip:port/RecruitAction/Leader/AddLeader

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CellPhoneNo| string | 是 |手机 |
| IDCard| string | 否 |身份证|
| RealName| string | 是 |姓名|
| PersonIDCardPathList | array string | 否 | 身份证图片正面列表 |
| PersonIDCardPathOtherList | array string | 否 | 身份证图片反面列表 |
















#### _应答数据_ {#应答数据-}
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaderSysNo| int| 是 |领队编码|



