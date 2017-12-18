# 注册账号 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

注册账号

_**【应用场景】**_

注册账号

注：追加一个登录账号到指定的账户中。默认可根据UserSysNo匹配；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AddLoginIn

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| PersonSysNo | int | 否 | 人员系统编码 |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 密码（微信等方式登录可为空） |
| IsEnable | int | 否 | 是否启用 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



