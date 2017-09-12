# 获取党员思想汇报列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员思想汇报列表

_**【应用场景】**_

获取党员思想汇报列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Report/GetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyMemberReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  | 是 | 查询条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 系统编码 |
| ReportTitle | string | 是 | 主题 |
| ReportContent | string | 是 | 内容 |
| Remark | string | 否 | 备注 |



