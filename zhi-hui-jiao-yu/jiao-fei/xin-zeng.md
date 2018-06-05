# 新增缴费 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增缴费

_**【应用场景】**_

新增缴费

_**【接口地址】**_

[http://ip:port/StudentFeeAction/StudentFee/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddStudentFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| PaidName | Nvarchar\(50\) | 是 | 缴费名称 |
| SubPaidClassCode | Nvarchar\(50\) | 是 | 子费种编码\(通用类\) |
| SubPaidClassName | Nvarchar\(50\) | 是 | 子费种名称 |
| PaidAmount | decimal\(18,2\) | 是 | 单笔缴费费用 |
| PaidStartDate | string | 否 | 有效期开始时间 |
| PaidEndDate | string | 否 | 有效期结束时间 |
| Remark | string | 否 | 备注 |
| PickRuleTemplateList | array object | 是 | 选人规则 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费编码 |



