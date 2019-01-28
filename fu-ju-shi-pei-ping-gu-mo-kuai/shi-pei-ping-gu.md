# 适配评估

_**【接口地址】**_

http://ip:port/FJAction/Adaption/Assess

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| adapType | int | 否 | 适配类型 |
| AssessSysNo | int | 是 | 评估id |
| AssessPersonSysNo | int | 是 | 评估人编码 |
| AssistSysNoList | array int | 否 | 所选辅具id |
| height | decimal | 否 | 身高 |
| weight | decimal | 否 | 体重 |
| living | valueData | 否 | 生活 |
| livingTime | valueData | 否 | 生活时间 |
| diseases | array valueData | 否 | 疾病诊断数组 |
| bedsores | array valueData | 否 | 危险因子数组 |
| others | array valueData | 否 | 其他医疗数组 |
| mainUsage | array string | 否 | 主要使用需求 |
| usage | string | 否 | 使用需求 |
| purpose | string | 否 | 使用目的 |
| menv1 | string | 否 | 主要环境 |
| menv2 | string | 否 | 主要环境里有 |
| senv1 | string | 否 | 次要环境 |
| senv2 | string | 否 | 次要环境里有 |
| assistance | string | 否 | 目前使用辅具 |
| usetime | valueData | 否  | 使用时间 |
| suit | string | 否 | 适合 |

valueData

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| id | int | 是 | id |
| name | string | 是 | 名称 |
| value | object | 否 | 值 |
| option | string | 否 | 选项 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupTitle | string | 是 | 组名 |
| QuestionList | array Question | 是 | 问题数组 |

Question

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionSysNo | int | 是 | 问题id |
| Question | string | 是 | 问题内容 |
| QuestionType | int | 是 | 1单选，2多选，3填空 |
| AnswerList | array Answer | 是 | 答案数组 |

Answer

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AnswerSysNo | int | 是 | 答案id |
| Answer | string | 是 | 答案文本 |
| AnswerType | int | 是 | 1文本，2图片，3语音 |
| Urls | array Answer | 是 | 资源链接 |