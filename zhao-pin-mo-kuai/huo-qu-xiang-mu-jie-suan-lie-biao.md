# 获取合同列表

##### _【功能说明】_ {#【功能说明】}

获取合同列表

_**【应用场景】**_

获取合同列表

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetSettlementList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementSysNo | int | 是 | 项目结算系统编码 |
| SettlementDate| string| 是 | 考勤月份 |
| OrganizationSysNo| int | 是 |所有者组织系统编码|
| ShopCount| int | 是 | 门店数 |
| WorkHour| int | 是 |工作小时数合计 |
| OvertimeHour| int | 是 | 固定加班小时数|
| ServiceCharge| decimal| 是 |服务费合计|
| TaxRate| decimal| 是 |税点|
| TotalAmount| decimal| 是 |开票金额|
| ActualAmount| decimal| 是 |实收金额|
| TotalStatus| int | 是 | 状态（0草稿，1已提交，2考勤已发放（待员工核对）， 3部分员工核对，4全部员工核对（待回款），5已回款，11平台退回，12员工退回，10已发薪水） |

