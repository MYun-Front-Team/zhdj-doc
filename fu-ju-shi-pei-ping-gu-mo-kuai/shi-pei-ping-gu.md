# 适配评估

_**【接口地址】**_

http://ip:port/FJAction/Adaption/Assess

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int | 是 | 评估id |
| AssessPersonSysNo | int | 是 | 审核人编码 |
| height | decimal | 否 | 身高 |
| weight | decimal | 否 | 体重 |
| menv1 | string | 否 | 主要环境 |
| menv2 | string | 否 | 主要环境里有 |
| senv1 | string | 否 | 次要环境 |
| senv2 | string | 否 | 次要环境里有 |
| diseases | array | 否 | 疾病诊断数组 |
| bedsores | array | 否 | 危险因子数组 |
| others | array | 否 | 其他医疗数组 |
| usage | string | 否 | 使用需求 |
| purpose | string | 否 | 使用目的 |
| assistance | string | 否 | 目前使用辅具 |
| usetime | string | 否  | 使用时间 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionList | array Question | 是 | 问题数组 |
