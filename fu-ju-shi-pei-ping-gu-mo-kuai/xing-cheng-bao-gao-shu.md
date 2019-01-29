# 形成报告书

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddReport

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int | 是 | 评估id |
| Diagnosis | string | 是 | 辅具相关诊断及医疗情况 |
| Requirement | string | 是 | 使用需求评估 |
| Physiology | string | 是 | 生理功能与构造评估 |
| Proposal | string | 否 | 辅具适配建议 |
| Summary | string | 否 | 辅具配置总结 |
| FJSysNoList | array int | 是 | 推荐辅具列表 |
| AssistantSysNoList | array int | 是 | 推荐产品列表 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 报告id |