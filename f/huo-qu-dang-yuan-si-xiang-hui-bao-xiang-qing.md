# 获取汇报详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取汇报详情

_**【应用场景】**_

获取汇报详情

_**【接口地址】**_

[http://ip:port/UMQuery/Report/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ReportBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 汇报系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 系统编码 |
| ReportTime | string | 是 | 汇报时间 |
| ReportTitle | string | 是 | 主题 |
| ReportContent | string | 是 | 内容 |
| Remark | string | 否 | 备注 |



