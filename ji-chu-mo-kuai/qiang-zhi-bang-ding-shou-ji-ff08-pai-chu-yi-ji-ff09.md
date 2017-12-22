# 强制绑定手机 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

强制绑定手机

_**【应用场景】**_

重新绑定手机登录账号，应用于手机更换后，登录账号也期望更换的需求场景；

注：该接口会注销原手机号的登录账号，并修改人员中的绑定手机，并创建新的手机登录账号；

注：验证后，验证码失效。

注：如果是客户自行重置，需验证旧手机号短信验证码，如果旧手机号已经无效，那么联系系统管理员重置；





_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/ReForceS](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etCellPhoneNoLoginID

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OldCellPhoneNo | string | 是 | 旧手机号 |
| NewCellPhoneNo | string | 是 | 新手机号 |
| Captcha | string | 是 | 新手机验证码 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |



