# 投票结果报表

##### _【功能说明】_ {#【功能说明】}

投票结果报表

_**【应用场景】**_

投票结果报表
_**【接口地址】**_

http://ip:port/VoteQuery/Vote/GetVoteReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 活动系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机号 |
| Propertys | array Propertys | 否 | 报表明细 |


#### VoteReportItem说明 {#应答数据-（巡河记录数组）}
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertySysNo | int | 否 | 投票主表编码 |
| PropertyValues | array[PropertyValue] | 否 | 投票主表编码 |


#### PropertyValue说明 {#应答数据-（巡河记录数组）}
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertyValueSysNo | int | 否 | 投票从表编码 |
| PropertyValue | int | 否 | 投票从表值 |






