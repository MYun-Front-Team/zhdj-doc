# 完善居民资料 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

完善居民资料

_**【应用场景】**_

完善居民资料

注：通过Person的PersonSysNo或者UserSysNo匹配到人，然后更新人员表和居民表数据；

当居民表中无该人数据时，新增一条记录；

_**【接口地址】**_

[http://ip:port/ResidentAction/Resident/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditResident

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 否 | 人员实体 |
|  |  |  | 其它居民字段暂不处理 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSysNo | int | 是 | 居民系统编码 |



