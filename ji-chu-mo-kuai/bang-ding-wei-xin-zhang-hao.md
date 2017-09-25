# 绑定微信账号 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

绑定微信账号

_**【应用场景】**_

绑定微信账号。

注：通过手机号找到Person，然后对应找到User，最后创建一个新的微信登录账号（需判断是否已经绑定过）

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etLoginInOpenId

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名（微信OpenID） |
| CellPhoneNo | string | 是 | 手机号 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |

#### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（即AdminSysNo） |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~是~~ | ~~数据范围枝叶列表~~ |
| Person | object | 是 | 人员实体对象 |



