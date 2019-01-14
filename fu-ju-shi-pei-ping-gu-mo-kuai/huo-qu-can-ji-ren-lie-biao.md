# 获取残疾人列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/FJQuery/Adaption/GetDisabledPersonList](http://ip:port/WTQuery/Water/GetWaterTankList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keyword | string | 否 | 关键字 |
| AreaCode | string | 否 | 区域编号 |
| DisabledType | int | 否 | 残疾类型 |
| DisabledLevel | int | 否 | 残疾等级 |



> #### _应答数据_ {#应答数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员id |
| AdminSysNo | int | 是 | 用户id |
| Name | string | 是 | 姓名 |
| Gender | int | 是 | 1男，2女 |
| Birthday | datetime | 是 | 生日 |
| CellPhoneNo | string | 是 | 手机 |
| IDNo | string | 是 | 身份证号 |
| DisabledNo | string | 是 | 残疾人证 |
| DisabledType | int | 是 | 残疾类型 |
| DisabledLevel | int | 是 | 残疾等级 |
| CellPhoneNo | string | 是 | 手机 |
| CellPhoneNo | string | 是 | 手机 |
| CellPhoneNo | string | 是 | 手机 |
| CellPhoneNo | string | 是 | 手机 |
| CellPhoneNo | string | 是 | 手机 |
| CellPhoneNo | string | 是 | 手机 |
| ContactPerson | string | 是 | 负责人 |
| ContactPhone | string | 是 | 联系电话 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| WaterTankNum | int | 是 | 水箱数量 |



