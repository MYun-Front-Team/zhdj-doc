# 获取居民详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取居民详情

_**【应用场景】**_

获取居民详情

注：当需要获取自己的居民信息时，IsOwner=1，通过UserSysNo匹配到人员后，获取居民信息。

_**【接口地址】**_

[http://ip:port/ResidentQuery/Resident/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ResidentBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSysNo | object | 是 | 居民系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| IsOwner | int | 否 | 是否获取自己的党员信息（1是） |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentBase | object | 是 | 基础字段 |
| ResidentStatistic | object | 否 | 统计字段 |



