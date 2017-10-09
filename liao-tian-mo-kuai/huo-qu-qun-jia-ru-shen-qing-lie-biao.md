# 获取群加入申请列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取群加入申请列表

_**【应用场景】**_

获取群加入申请列表

注：这里的计算字段是以申请人为准。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupJoinList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 否 | 群系统编码 |
| Query | object | 是 | 搜索条件 |
| Limit | object | 否 | 限制条件 |

> #### Sorts说明 \(数组\) {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsDescending | int | 是 | 是否倒序：0否，1是 |
| Name | string | 是 | 排序字段名称：如时间CreateTime，其它见模块说明 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupJoinSysNo | int | 是 | 群加入申请编码 |
| GroupSysNo | int | 是 | 群系统编码 |
| Person | object | 是 | 成员实体（见基础模块登录） |
| JoinStatus | int | 是 | 加入状态：0申请中，1加入，2拒绝 |
| JoinReason | string | 否 | 申请理由 |
| RefuseReason | string | 否 | 拒绝理由 |
| GroupStatistic | object | 是 | 计算字段\(见模块说明\) |



