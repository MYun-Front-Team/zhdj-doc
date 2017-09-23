# 校验验证码 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

校验验证码

_**【应用场景】**_

校验验证码

注：保留验证码的有效性。

_**【接口地址】**_

[http://ip:port/UMAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Captcha](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/CheckCaptcha](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CellPhoneNo | string | 是 | 手机号 |
| CaptchaType | int | 是 | 验证码类型：1注册验证码，2激活验证码，3重置密码，4修改手机，5绑定微信 |
| Captcha | string | 是 | 验证码 |



