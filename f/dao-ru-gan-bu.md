# 导入干部

_**【接口地址】**_

http://ip:port/PartyAction/Party/ImportCadre

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataList | array object | 是 | 干部列表 |

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

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



