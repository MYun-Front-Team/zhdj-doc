# 新增干部

_**【接口地址】**_

http://ip:port/PartyAction/Party/AddCadre

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
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
| MaritalStatus | int | 否 | 婚姻状况 |
| HousingStatus | int | 否 | 住房情况 |
| BusinessStatus | int | 否 | 本人是否经商 |
| BusinessReason | string | 否 | 经商说明 |
| ContractAddress | string | 否 | 家庭住址 |
| PersonIDPhotoPathList | array string | 否 | 证件照图片列表 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 干部id |



