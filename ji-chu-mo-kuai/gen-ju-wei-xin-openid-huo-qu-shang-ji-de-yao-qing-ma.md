#根据微信OPENID获取上级的邀请码

##### _【功能说明】_ {#【功能说明】}

根据微信OPENID获取上级的邀请码

_**【应用场景】**_

根据微信OPENID获取上级的邀请码

_**【接口地址】**_
http://ip:port/BasicQuery/Basic/GetBizCompanyCodeBySaasKey

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WxOpenID| string | 是 | WxOpenID |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InvitationCode| string | 是 | 上级邀请码 |



