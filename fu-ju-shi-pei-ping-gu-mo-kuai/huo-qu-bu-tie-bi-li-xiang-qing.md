# 获取补贴比例详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaptation/GetSubsidyTypeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | id |

> ####  {#应答数据-（巡河记录数组）}

SubsidyType

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | id |
| AreaCode | int | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| SubsidyTypeName | string | 是 | 补贴人群类别名称 |
| Ratio | decimal | 是 | 比例 |
| PersonSysNo | int | 是 | 创建人id |
| PersonName | string | 是 | 创建人 |
| CreateTime | datetime | 是 | 创建时间 |



