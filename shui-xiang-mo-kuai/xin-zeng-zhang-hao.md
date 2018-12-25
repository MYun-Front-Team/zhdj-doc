# 新增账户 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTAction/Water/AddUser](http://ip:port/WTAction/Water/AddUser)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationType | int | 是 | 17031小区负责人，17032小区物业，17033水务局 |
| PersonName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机号 |
| Password | string | 是 | 密码 |
| UserGender | int | 是 | 1男，2女 |
| HouseEstateSysNoList | array int | 是 | 负责小区id列表 |



#### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 用户id |



