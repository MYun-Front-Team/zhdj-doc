# 获取残疾人列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetDisabledPersonList

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



