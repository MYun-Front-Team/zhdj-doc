# 残疾人注册

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddDisabledPerson

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CellPhoneNo | string | 是 | 手机号 |
| Password | string | 是 | 密码 |
| Name | string | 是 | 姓名 |
| IDNo | string | 是 | 身份证号 |
| AreaCode | string | 是 | 区域编号 |
| DisabledNo | string | 是 | 残疾证号 |
| DisabledType | int | 是 | 残疾类型 |
| DisabledLevel | int | 是 | 残疾等级 |
| State | int | 是 | 1有效，0注销 |

> #### _应答数据_


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 人员id |





