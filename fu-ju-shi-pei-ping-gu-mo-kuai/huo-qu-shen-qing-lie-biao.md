# 获取申请列表

_**【接口地址】**_

[http://ip:port/FJQuery/Adaptation/GetApplyList](http://ip:port/FJQuery/Adaptation/GetDisabledPersonList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Name | string | 否 | 姓名 |
| IDNo | string | 否 | 身份证号 |
| DisabledType | int | 否 | 残疾类别 |
| DisabledLevel | int | 否 | 残疾等级 |
| AreaCode | string | 否 | 区域编号 |

> ####  {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |
| PersonSysNo | int | 是 | 人员系统编码 |
| AdminSysNo | int | 是 | 用户系统编码 |
| Name | string | 是 | 姓名 |
| Gender | int | 是 | 1男，2女 |
| Age | int | 是 | 年龄 |
| CellPhoneNo | string | 是 | 手机号 |
| IDNo | string | 是 | 身份证号 |
| DisabledNo | string | 是 | 残疾证号 |
| DisabledType | int | 是 | 残疾类型 |
| DisabledLevel | int | 是 | 残疾等级 |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| State | int | 是 | 1有效，0注销 |
| AvatarUrl | string | 是 | 头像 |
| ApplyCode | string | 是 | 申请单编号 |
| ApplyTime | datetime | 是 | 申请时间 |
| ApplyPersonSysNo | int | 是 | 申请人编码 |
| ApplyStatus | int | 是 | 1待评估，2待村社区审核，3待乡镇街道审批，4待区县审批，5待市级审批，6待省级审批，10已完成，11已退回 |
| SubsidyTypeList | array SubsidyType | 是 | 符合补贴人群类别列表 |
| AssistantType | int | 是 | 申请辅助器具类别 |
| ApplyRemark | string | 是 | 申请辅助器具说明 |
| HandleLogList | array HandleLog | 是 | 处理流程列表 |
| WaitHandleList | array WaitHandle | 是 | 待处理信息列表 |

SubsidyType

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | 符合补贴人群类别id |
| SubsidyTypeName | string | 是 | 符合补贴人群类型名称 |

HandleLog

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |
| HandleType | int | 是 | 1评估，2村社区审核，3乡镇街道审批，4区县审批，5市级审批，6省级审批 |
| HandleResult | int | 是 | 10通过\(或已评估\)，11拒绝 |
| HandleTime | datetime | 是 | 处理时间 |
| HandlePersonSysNo | int | 是 | 操作人id |
| HandlePersonName | string | 是 | 操作人姓名 |
| HandleRemark | string | 是 | 处理意见 |
| AssessmentSysNo | int | 是 | 评估id |
| ReportSysNo | int | 是 | 报告书id |

WaitHandle

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HandleType | int | 是 | 1适配评估，2村社区审核，3乡镇街道审批，4区县审批，5市级审批，6省级审批 |
| WaitHandlePersonSysNo | int | 是 | 未处理人id |
| WairHandlePersonName | string | 是 | 未处理人姓名 |
| SortNo | int | 是 | 排序 |



