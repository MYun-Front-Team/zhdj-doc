# 获取申请列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetApplyList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keyword | string | 否 | 关键字 |
| Name | string | 否 | 姓名 |
| IDNo | string | 否 | 身份证号 |
| DisabledNo | string | 否 | 残疾人证号 |
| AreaCode | string | 否 | 区域编号 |
| DisabledType | int | 否 | 残疾类型 |
| DisabledLevel | int | 否 | 残疾等级 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |
| ApplyCode | string | 是 | 申请编号 |
| ApplyTime | datetime | 是 | 申请时间 |
| ApplyPersonSysNo | int | 是 | 申请人编码 |
| ApplyPerson | string | 是 | 申请人 |
| ApplyStatus | int | 是 | 1待评估，2待村社区审核，3待乡镇街道审批，4待区县审批，5待市级审批，6待省级审批，10已完成，11已退回 |
| PersonSysNo | int | 是 | 人员id |
| AdminSysNo | int | 是 | 用户id |
| Name | string | 是 | 姓名 |
| AvatarUrl | string | 是 | 头像 |
| Gender | int | 是 | 1男，2女 |
| Birthday | datetime | 是 | 生日 |
| Age | int | 是 | 年龄 |
| CellPhoneNo | string | 是 | 手机 |
| IDNo | string | 是 | 身份证号 |
| DisabledNo | string | 是 | 残疾人证号 |
| DisabledType | int | 是 | 残疾类型 |
| DisabledLevel | int | 是 | 残疾等级 |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| State | int | 是 | 1有效，0注销 |
| Nation | string | 是 | 民族 |
| Education | string | 是 | 学历 |
| Profession | string | 是 | 职业 |
| ContactPerson | string | 是 | 联系人 |
| ContactPhone | string | 是 | 联系电话 |
| Relation | string | 是 | 关系 |
| HomeAreaCode | string | 是 | 家庭区域编号 |
| HomeAreaName | string | 是 | 家庭区域名称 |
| Address | string | 是 | 具体地址 |
| Postalcode | string | 是 | 邮政编码 |
| Email | string | 是 | 电子邮件 |
| AssistantType | int | 是 | 申请辅助器具类别id |
| AssistantTypeName | string | 是 | 申请辅助器具类别 |
| ApplyRemark | string | 是 | 申请辅助器具说明 |
| SubsidyTypeList | array SubsidyType | 是 | 符合补贴人群类别列表 |
| HandleLogList | array Handlelog | 是 | 处理流程列表 |
| WaitHandleList | array WaitHandle | 是 | 待处理信息列表 |

SubsidyType

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | 补贴id |
| SubsidyTypeName | string | 是 | 补贴名称 |
| Ratio | decimal | 是 | 补贴比例 |

HandleLog

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |
| HandleType | int | 是 | 1评估，2村社区审核，3乡镇街道审批，4区县审批，5市级审批，6省级审批 |
| HandleResult | int | 是 | 10通过(或已评估)，11拒绝 |
| HandleTime | datetime | 是 | 处理时间 |
| HandlePersonSysNo | int | 是 | 操作人id |
| HandlePersonName | string | 是 | 操作人 |
| HandleRemark | string | 是 | 处理意见 |
| AssessmentSysNo | int | 是 | 评估id |
| ReportSysNo | int | 是 | 报告书id |

WaitHandle

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HandleType | int | 是 | 1评估，2村社区审核，3乡镇街道审批，4区县审批，5市级审批，6省级审批 |
| HandlePersonSysNo | int | 是 | 处未理人id |
| HandlePersonName | string | 是 | 未处理人 |

