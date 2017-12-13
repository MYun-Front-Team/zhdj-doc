# 注册账户 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

注册账户

_**【应用场景】**_

注册账户

注：“账户”是指一个新人首次使用系统时需要注册的操作。

当登录类型=0（手机号）时，需判断是否存在Person，否则新增。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Register](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 密码（微信等方式登录可为空） |
| PersonName | string | 否 | 昵称/真实姓名（同时填充） |
| UserGender | int | 否 | 性别：1男，2女 |
| FilePathList | array string | 否 | 头像Path路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（即AdminSysNo） |



