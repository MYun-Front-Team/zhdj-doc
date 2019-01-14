# 获取补贴类目详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetAssistantTypeBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantTypeSysNo | int | 是 | 类目id |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantTypeSysNo | int | 是 | 类目id |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| CategorySysNo | int | 是 | 辅具类别编码 |
| CategoryName | string | 是 | 辅具类别名称 |
| AssistantTypeName | string | 是 | 类目名称 |
| Year | int | 是 | 申请年限 |
| NeedAssess | int | 是 | 1需要评估，0不需要评估 |
| Standard | string | 是 | 补贴标准 |
| PersonSysNo | int | 是 | 创建人id |
| PersonName | string | 是 | 创建人 |
| CreateTime | datetime | 是 | 创建时间 |





