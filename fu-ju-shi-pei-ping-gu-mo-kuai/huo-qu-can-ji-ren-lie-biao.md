# 获取残疾人列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaptation/GetDisabledPersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> ####  {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
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
|  |  |  |  |



