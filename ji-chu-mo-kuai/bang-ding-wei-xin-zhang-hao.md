# 绑定微信账号 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

绑定微信账号

_**【应用场景】**_

绑定微信账号。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etLoginInOpenId

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 新密码 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |



