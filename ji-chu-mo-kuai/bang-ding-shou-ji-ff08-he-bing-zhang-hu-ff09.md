# 绑定手机（合并账户） {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

绑定手机

_**【应用场景】**_

绑定手机时如果遇到手机号已经被占用，那么该账户下的微信OPENID和微信登录账号将绑定到原占用手机的账户下。

注：如果原占用手机账户下已经存在微信数据，则提示手机号已占有；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/ReS](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etCellPhoneNoBindPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewCellPhoneNo | string | 是 | 新手机号 |
| Captcha | string | 是 | 验证码 |

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReSetStatus | int | 是 | 状态：1绑定成功，10占用成功（需重新登录），11绑定失败 |
| UserSysNo| int | 是 | UserSysNo |
| PersonSysNo| int | 是 | PersonSysNo|
| OrganizationList| array[Organization]| 是 | OrganizationList|













