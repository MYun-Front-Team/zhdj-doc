# 检查账号保护密码是否正确

##### _【功能说明】_ {#【功能说明】}

检查账号保护密码是否正确

_**【应用场景】**_

检查账号保护密码是否正确

_**【接口地址】**_

http://ip:port/RecruitQuery/Wallet/CheckNPLWallet

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PassWord | string | 是 | 密码|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NPLWalletStatus | int | 是 | 状态(0无密码，11密码错误，10密码正确) |




