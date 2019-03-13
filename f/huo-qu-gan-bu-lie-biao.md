# 获取干部列表

_**【接口地址】**_

http://ip:port/PartyQuery/Party/GetCadreList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keyword | string | 否 | 关键字 |
| DataRangeSysNoList | array int | 否 | 行政区划 |
| EducationList | array int | 否 | 学历 |
| InnerPartyStatusList | array int | 否 | 政治面貌 |
| Awarded | int | 否 | 是否获奖：0全部，1是，2否 |
| Punished | int | 否 | 是否受过处分：0全部，1是，2否 |


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

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 区划id |
| DataRangeName | string | 是 | 区划名称 |





