# 重置密码 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

重置密码

_**【应用场景】**_

重置密码。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/ReS](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etLoginInPwd

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginNewPwd | string | 是 | 新密码 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |



