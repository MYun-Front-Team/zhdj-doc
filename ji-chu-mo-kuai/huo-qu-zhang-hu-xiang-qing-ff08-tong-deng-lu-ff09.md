# 获取账户详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取账户详情

_**【应用场景】**_

获取账户详情

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etLoginResult

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目号 |
| UserSysNo | int | 否（二选一） | 用户系统编码（同Admin） |
| PersonSysNo | int | 否（二选一） | 人员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

同登录返回结果；

