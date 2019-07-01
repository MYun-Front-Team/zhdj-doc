# 上传考勤表

##### _【功能说明】_ {#【功能说明】}

上传考勤表

_**【应用场景】**_

上传考勤表

_**【接口地址】**_

http://ip:port/RecruitAction/Settlement/AddSettlement 
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Settlement|SettlementAdd| 否 | 项目表头 |
| SettlementItems|array[SettlementItemAdd]| 否 | 项目明细 |


#### SettlementAdd

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementDate| string| 是 | 考勤月份开始|
| SettlementDateEnd| string| 是 | 考勤月份结束 |
| OrganizationSysNo| int | 是 |所有者组织系统编码|

#### SettlementItemAdd

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Index| int| 是 |行号（1开始） |
| RealName| string| 是 | 人员名称|
| CellPhoneNo| string| 是 | 手机号|
| OrganizationSysNo| int | 是 | 组织系统编码 |
| ShopName| string| 是 |店铺名称 |
| Salary| decimal | 是 |时薪水 |
| EntryDate| datetime| 是 |入职时间 |
| QuitDate| datetime| 是 |离职时间 |
| SellerReward | decimal| 是 |商家奖励金|
| SellerFine| decimal| 是 |商家罚款|
| WorkHour| int | 是 |工作小时数合计 |
| OvertimeHour| int | 是 |固定加班小时数 |
|GZOvertimeHour | int | 否 | 工作日加班时小时数 |
| GXOvertimeHour| int | 否 | 公休日加班时小时数 |

#### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | | 是 |项目表系统编码 |

