# 获取党员发展统计 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员发展统计

_**【应用场景】**_

获取党员发展统计

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyDevelopStatistics

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| DevelopStartDate | string | 是 | 发展开始时间 |
| DevelopEndDate | string | 是 | 发展结束时间 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberInfos | array object | 是 | 党员党内状态统计（见党建机构地图说明） |



