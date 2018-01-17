# 重新绑定手机 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

重新绑定手机

_**【应用场景】**_

重新绑定手机。

注：该接口不会注销原手机号的登录账号。只修改人员中的绑定手机。

注：验证后，验证码失效。

注：当IsCreateLogin=1时，先判断该手机号是否已被创建账号。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/ReS](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etCellPhoneNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewCellPhoneNo | string | 是 | 新手机号 |
| Captcha | string | 是 | 验证码 |
| IsCreateLogin | int | 否 | 是否创建手机账号：0否，1是 |
| LoginSource | int | 否 | 登录来源（枚举） |
| LoginType | int | 否 | 登录类型（枚举） |



