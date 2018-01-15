# 获取项目请求地址 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取项目请求地址

_**【应用场景】**_

获取项目请求地址

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RequestUrl

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| RequestType | int | 否 | 请求类型 |
| RequestSource | int | 是 | 请求来源：1PC，2APP，3H5，4微信 |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RequestUrl | string | 是 | 请求地址 |



