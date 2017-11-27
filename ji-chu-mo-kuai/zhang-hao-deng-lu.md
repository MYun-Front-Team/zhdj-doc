# 账号登录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

账号登录

_**【应用场景】**_

账号登录，密码在特殊登录方式可为空，登录成功后，需要更新账户表的最后登录时间。其它账户的登录数据（如登录设备、Token等）需调用修改账户接口。

注：需判断账户是否已经激活，账号是否停用。

积分备注：登录动作（枚举=2）预埋积分赠送逻辑。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/L](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)oginIn

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 密码（微信等方式登录可为空） |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（即AdminSysNo） |
| User | object | 是 | 账户实体对象 |
| Person | object | 是 | 人员实体对象 |
| OrganizationList | array object | 是 | 组织列表 |

#### Person说明_ （简要，需要全部字段请调用“获取个人信息”接口）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PersonAge | int | 否 | 年龄 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| ~~Post~~ | ~~string~~ | ~~否~~ | ~~工作岗位~~ |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |

#### User说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（即AdminSysNo） |
| LastLoginDate | string | 否 | 上一次登录时间 |
| DeviceType | int | 否 | 设备类型：1IOS，2安卓，3小米，4华为 |
| DeviceToken | string | 否 | 设备Token |
| WxOpenID | string | 否 | 微信Openid |

#### Organization说明_ （简要，需要全部字段请调用“获取组织信息”接口）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| OrganizationType | int | 是 | 类型（枚举） |
| OrganizationClassSysNo | int | 否 | 分类（树） |
| OrganizationName | string | 是 | 组织名称 |
| OrganizationShortName | string | 否 | 组织简称 |



