# 新增会员卡（按PersonSysNo）

##### _【功能说明】_ {#【功能说明】}

新增会员卡（按PersonSysNo）

_**【应用场景】**_
新增会员卡（按PersonSysNo）


_**【接口地址】**_

http://ip:port/WalletAction/MemberCard/AddPersonMemberCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 是 |人员系统编码|
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡，3学生考勤卡，4学生一卡通 |
| CardNo | string | 是 | 卡号 |
| CardKey | string | 否 | 卡密码 |
| CardPhoneNo | string | 否 | 手机号 |
| IDCard | string | 否 | 身份证 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo | int | 是 | 系统编码 |



