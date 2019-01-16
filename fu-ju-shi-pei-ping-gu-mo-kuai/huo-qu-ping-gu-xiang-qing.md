# 获取评估详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetAssessBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int | 是 | 评估id |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int | 是 | 评估id |
| AssessCode | string | 是 | 评估编号 |
| AssessTime | datetime | 是 | 评估时间 |
| AssessPersonSysNo | int | 是 | 评估人编码 |
| AssessPerson | string | 是 | 评估人 |
| ApplySysNo | int | 是 | 申请id |
| ApplyCode | string | 是 | 申请编号 |
| ApplyPersonSysNo | int | 是 | 申请人编码 |
| ApplyPerson | string | 是 | 申请人 |
| ApplyTime | datetime | 是 | 申请时间 |
| AssessStatus | int | 是 | 1待评估，2评估中，10已评估，11已作废 |
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

SubsidyType

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | 补贴id |
| SubsidyTypeName | string | 是 | 补贴名称 |
| Ratio | decimal | 是 | 补贴比例 |





