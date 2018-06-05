# 修改缴费 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改缴费

_**【应用场景】**_

修改缴费

注：未审核通过的缴费记录都允许修改，如审核失败的缴费修改后，审核状态初始化；

_**【接口地址】**_

[http://ip:port/StudentFeeAction/StudentFee/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditStudentFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费系统编码 |
| PaidName | Nvarchar\(50\) | 是 | 缴费名称 |
| SubPaidClassCode | Nvarchar\(50\) | 是 | 子费种编码\(通用类\) |
| SubPaidClassName | Nvarchar\(50\) | 是 | 子费种名称 |
| PaidAmount | decimal\(18,2\) | 是 | 单笔缴费费用 |
| PaidStartDate | string | 否 | 有效期开始时间 |
| PaidEndDate | string | 否 | 有效期结束时间 |
| Remark | string | 否 | 备注 |
| PickRuleTemplateList | array object | 是 | 选人规则 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



