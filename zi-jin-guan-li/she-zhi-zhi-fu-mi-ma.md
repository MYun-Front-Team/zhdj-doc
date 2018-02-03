# 设置支付密码 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置支付密码

_**【应用场景】**_

设置支付密码

注：PersonSysNo=0则通过操作人获取。

_**【接口地址】**_

[http://ip:port/WalletAction/Wallet/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etOrgPayPassword

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| PayPassword | string | 是 | 支付密码 |
| CellphoneNo | string | 是 | 手机号 |
| Captcha | string | 是 | 验证码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



