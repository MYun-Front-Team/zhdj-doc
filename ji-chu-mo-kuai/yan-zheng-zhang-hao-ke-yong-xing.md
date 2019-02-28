# 验证账号可用性 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

验证账号可用性

_**【应用场景】**_

验证账号可用性

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/C](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)heckLoginInStatus

注：账号不存在，只需要判断账号是否存在；

账号已存在分二种情况：

1、密码为空；

2、账号和密码不一致；

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 密码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginInStatus | int | 是 | 状态：0账号不存在，1账号已存在未激活（密码为空），2账号正常，3账号被禁用 |



