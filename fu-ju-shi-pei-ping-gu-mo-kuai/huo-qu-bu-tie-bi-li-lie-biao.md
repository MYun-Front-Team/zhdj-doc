# 获取补贴比例列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetSubsidyTypeList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeName | string | 否 | 补贴人群类别 |
| AreaCode | string | 否 | 区域编号 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | 补贴比例id |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| SubsidyTypeName | string | 是 | 补贴人群类别 |
| Ratio | decimal | 是 | 比例 |
| PersonSysNo | int | 是 | 创建人id |
| PersonName | string | 是 | 创建人 |
| CreateTime | datetime | 是 | 创建时间 |





