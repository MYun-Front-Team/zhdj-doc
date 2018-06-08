# 新增会员卡 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增会员卡

_**【应用场景】**_

新增会员卡

注：1、金额与组织关联，激活状态下开卡金额要充值到组织钱包中，并留有log日志；

2、会员卡类型，必须传手机号，并通过手机号找到所在人的组织；

3、找不到匹配组织的新卡，需新增一个组织和人；

4、判断该卡号是否已经激活，如果激活则提示不允许重复激活；如果状态为未激活则修改，否则新增； 同一个卡号不允许绑定在不同的组织上；

_**【接口地址】**_

[http://ip:port/WalletAction/MemberCard/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddMemberCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡，3学生考勤卡 |
| CardNo | string | 是 | 卡号 |
| CardKey | string | 是 | 卡密码 |
| CardPhoneNo | string | 否 | 手机号 |
| IDCard | string | 否 | 身份证 |
| CardAmount | decimal（18，2） | 是 | 开卡金额 |
| IsActivity | int | 否 | 是否激活：0否，1是 |
| GiveAmount | decimal（18，2） | 否 | 赠送金额 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo | int | 是 | 系统编码 |
| User | int | 否 | 账户 |
| RechargeSysNo | int | 否 | 充值系统编码 |



