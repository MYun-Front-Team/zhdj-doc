# 获取乡级列表

_**【接口地址】**_

[http://ip:port/UMQuery/Area/GetStreets](http://ip:port/UMQuery/Area/GetAreas)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AreaCode | string | 否 | 县级编号 |

> #### PriceGroup {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo | int | 是 | 系统编码 |
| Code | string | 是 | 编号 |
| Name | string | 是 | 名称 |
| AreaCode | string | 是 | 县级编号 |
| CityCode | string | 是 | 地级编号 |
| ProvinceCode | string | 是 | 省级编号 |



