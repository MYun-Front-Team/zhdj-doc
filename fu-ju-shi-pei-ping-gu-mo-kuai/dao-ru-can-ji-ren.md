# 导入残疾人

_**【接口地址】**_

http://ip:port/FJAction/Adaption/ImportDisabledPerson

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DisabledList | array ImportDisabled | 是 | 残疾人列表 |

ImportDisabled

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Name | string | 是 | 姓名 |
| Gender | int | 是 | 1男，2女 |
| Birthday | datetime | 是 | 生日 |
| CellPhoneNo | string | 是 | 手机 |
| IDNo | string | 是 | 身份证号 |
| DisabledNo | string | 是 | 残疾人证号 |
| DisabledType | int | 是 | 残疾类型 |
| DisabledLevel | int | 是 | 残疾等级 |
| AreaName | string | 是 | 区域名称 |
| Nation | string | 是 | 民族 |
| Education | string | 是 | 学历 |
| Profession | string | 是 | 职业 |
| ContactPerson | string | 是 | 联系人 |
| ContactPhone | string | 是 | 联系电话 |
| Relation | string | 是 | 关系 |
| HomeAreaName | string | 是 | 家庭区域名称 |
| Address | string | 是 | 具体地址 |
| Postalcode | string | 是 | 邮政编码 |
| Email | string | 是 | 电子邮件 |



> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




