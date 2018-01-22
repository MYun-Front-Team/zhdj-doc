# 获取巡房记录详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取巡房记录详情

_**【应用场景】**_

获取巡房记录详情

注：“PatrolHouseSysNo"和”GridManSysNo“，”HouseSysNo“ 二选一必填；

”GridManSysNo“，”HouseSysNo“只需要查询正在巡房的PatrolHouseSysNo；

_**【接口地址】**_

[http://ip:port/ResidentQuery/House/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PatrolHouseBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PatrolHouseSysNo | int | 是（二选一） | 巡房记录系统编码 |
| GridManSysNo | int | 否（二选一） | 网格员系统编码 |
| HouseSysNo | int | 否（二选一） | 房屋系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| House | object | 是 | 房屋实体（简版） |
| GridMan | object | 是 | 网格员实体（简版） |
| PatrolDate | string | 是 | 巡查日期 |
| PatrolStartDate | string | 是 | 巡查开始时间 |
| PatrolEndDate | string | 否 | 巡查结束时间 |
| PatrolCompareLogList | array object | 否 | 巡查对照日志列表 |



