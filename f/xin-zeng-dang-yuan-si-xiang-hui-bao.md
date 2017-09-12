# 新增党员思想汇报 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增党员思想汇报

_**【应用场景】**_

新增党员思想汇报

_**【接口地址】**_

[http://ip:port/PartyAction/Report/AddP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyMemberReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| ReportTitle | string | 是 | 荣誉抬头 |
| ReportContent | string | 是 | 荣誉说明 |
| Remark | string | 否 | 备注 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 系统编码 |



