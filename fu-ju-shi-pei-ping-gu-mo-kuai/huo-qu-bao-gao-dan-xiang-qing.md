# 获取报告单详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetReportBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 否 | 报告书id |
| AssessSysNo | int | 否 | 评估id |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportSysNo | int | 是 | 报告id |
| AssessSysNo | int | 是 | 评估id |
| AssessCode | string | 是 | 评估编号 |
| AssessTime | datetime | 是 | 评估时间 |
| AssessPersonSysNo | int | 是 | 评估人编码 |
| AssessPerson | string | 是 | 评估人 |
| AssessStatus | int | 是 | 1待评估，10已评估，11已作废 |
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
| Diagnosis | string | 是 | 辅具相关诊断及医疗情况 |
| Requirement | string | 是 | 使用需求评估 |
| Physiology | string | 是 | 生理功能与构造评估 |
| Proposal | string | 是 | 辅具适配建议 |
| Summary | string | 是 | 辅具配置总结 |
| Suggest | string | 是 | 评估意见 |
| SelectAssistantSysNo | int | 是 | 选择辅具id |
| FJList | array FJ | 是 | 推荐辅具列表 |
| AssistantList | array Assistant | 是 | 推荐产品列表 |

FJ

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FJSysNo | int | 是 | 辅具id |
| ISO | string | 是 | ISO |
| FJName | string | 是 | 辅具名称 |
| IsMain | int | 是 | 1主件，0配件 |

Assistant

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantSysNo | int | 是 | 产品id |
| AssistantCode | string | 是 | 产品编号 |
| AssistantName | string | 是 | 产品名称 |
| BrandSysNo | int | 是 | 品牌id |
| BrandName | string | 是 | 品牌名称 |
| SupplierSysNo | int | 是 | 供应商id |
| SupplierName | string | 是 | 供应商名称 |