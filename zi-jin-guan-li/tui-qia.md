# 退卡 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

退卡

_**【应用场景】**_

退卡

注：1、当IsReturnAmount=1时，需清空该组织下钱包余额，并记录日志；

2、设置卡状态=0，并删除与组织关系；

3、验证手机号与开卡时的手机号一致；

4、无手机号的情况下，是退非会员卡，不允许退金额；

_**【接口地址】**_

[http://ip:port/WalletAction/MemberCard/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)MoveMemberCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardNo | string | 是 | 卡号 |
| IsReturnAmount | int | 是 | 是否退款：0否，1是 |
| CellPhoneNo | string | 否 | 手机号 |
| ~~CaptchaType~~ | ~~int~~ | ~~是~~ | ~~验证码类型：6验证手机号~~ |
| ~~Captcha~~ | ~~string~~ | ~~是~~ | ~~验证码~~ |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



