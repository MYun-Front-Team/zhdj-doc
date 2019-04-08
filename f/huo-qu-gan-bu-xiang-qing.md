# 获取干部详情

_**【接口地址】**_

http://ip:port/PartyQuery/Party/GetCadreBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 干部id |


#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 干部id |
| PersonSysNo | int | 是 | 人员id |
| DataRangeSysNo | int | 是 | 村社区 |
| MemberName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机 |
| MemberGender | int | 否 | 性别：1男，2女 |
| IDCard | string | 是 | 身份证 |
| BirthDay | datetime | 否 | 出生年月 |
| Education | int | 否 | 教育 |
| ShortNo | string | 否 | 短号 |
| Post | string | 否 | 职务 |
| InnerPartyStatus | int | 是 | 政治面貌 |
| PersonIDPhotoUrlList | array string | 否 | 证件照图片列表 |
| DataRangeList | array object | 否 | 区划列表 |
| AwardList | array object | 否 | 奖励列表 |
| PunishList | array object | 否 | 惩罚列表 |
| ReportList | array object | 否 | 报告列表 |
| RenMianList | array object | 否 | 任免列表 |
| LvZhiList | array object | 否 | 履职列表 |
| GeRenList | array object | 否 | 个人列表 |
| LogList | array object | 否 | 日志列表 |


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 区划id |
| DataRangeName | string | 是 | 区划名称 |


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| APSysNo | int | 是 | 奖惩id |
| MemberSysNo | int | 是 | 干部id |
| GeneralType | int | 是 | 1奖励，2惩罚，3重大事项报告 |
| Year | string | 是 | 年度 |
| Level | string | 否 | 级别 |
| AwardType | string | 否 | 获奖类型 |
| PunishType | string | 否 | 处分 |
| Report | string | 否 | 重大事项报告 |
| FileList | array object | 否 | 附件列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileName | string | 是 | 附件名称 |
| FileUrl | string | 是 | 附件路径 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserName | string | 是 | 修改人 |
| CreateTime | datetime | 是 | 修改时间 |
| ModifyKey | string | 是 | 修改类型名称 |
| OldValue | string | 是 | 原数值 |
| NewValue | string | 是 | 新数值 |


