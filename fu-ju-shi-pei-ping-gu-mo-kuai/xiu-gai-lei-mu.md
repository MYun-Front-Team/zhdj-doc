# 新增类目

_**【接口地址】**_

[http://ip:port/FJAction/Adaptation/EditAssistantType](http://ip:port/FJQuery/Adaptation/GetAssistantTypeBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantTypeSysNo | int | 是 | 类目id |
| AreaCode | int | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| CategorySysNo | int | 是 | 辅具类别id |
| AssistantTypeName | string | 是 | 类目名称 |
| Year | int | 是 | 申请年限 |
| NeedAssess | int | 是 | 1需要评估，0不需要评估 |
| Standard | string | 是 | 补贴标准 |

> ####  {#应答数据-（巡河记录数组）}

AssistantType

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |




