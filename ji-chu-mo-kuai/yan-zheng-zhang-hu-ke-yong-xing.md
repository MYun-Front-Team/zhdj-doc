# 验证账户可用性 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

验证账户可用性

_**【应用场景】**_

验证账户可用性

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/C](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)heckCellPhoneNoStatus

注：只验证手机号是否已经被其他人绑定；

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| CellPhoneNo | string | 否 | 密码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |



