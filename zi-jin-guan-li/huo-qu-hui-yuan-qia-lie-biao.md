# 获取会员卡列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取会员卡列表

_**【应用场景】**_

获取会员卡列表

_**【接口地址】**_

[http://ip:port/WalletQuery/MemberCard/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMemberCardList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 所属组织系统编码 |
| OrganizationToSysNo | int | 否 | 附属组织系统编码 |
| CardTypeList | int | 否 | 会员卡类型：0会员卡，1礼品卡，2临时卡 |
| CardNo | string | 否 | 卡号 |
| CardPhoneNo | string | 否 | 手机号 |
| IDCard | string | 否 | 身份证 |
| CardStatusList | int | 否 | 卡状态：0初始化，9已挂失，10已激活，11已删除 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCard | object | 是 | 会员卡 |
| Wallet | object | 是 | 钱包 |

#### MemberCard说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardSysNo | int | 是 | 会员卡系统编码 |
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡 |
| CardNo | string | 是 | 卡号 |
| CardPhoneNo | string | 否 | 手机号 |
| IDCard | string | 否 | 身份证 |
| CardAmount | decimal（18，2） | 是 | 开卡金额 |
| CardStatus | int | 否 | 卡状态：0初始化，9已挂失，10已激活，11已删除 |
| User | object | 否 | 账户 |



