# 新增小区 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTAction/Water/AddHouseEstate](http://ip:port/WTQuery/Water/GetWaterTankList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateName | string | 是 | 小区名称 |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |
| ContactPerson | string | 是 | 负责人 |
| ContactPhone | string | 是 | 联系电话 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 小区id |



