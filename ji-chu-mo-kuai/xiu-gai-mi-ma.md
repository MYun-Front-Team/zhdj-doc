# 修改密码 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改密码

_**【应用场景】**_

修改密码。

注：需判断账户是否已经激活，账号是否停用。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditLoginInPwd

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginOldPwd | string | 是 | 旧密码 |
| LoginNewPwd | string | 是 | 新密码 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |



