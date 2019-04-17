# 上肢辅具适配评估

_**【接口地址】**_

http://ip:port/FJAction/Adaption/UpperlimbAssess

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| adapType | int | 否 | 适配类型 |
| AssessSysNo | int | 是 | 评估id |
| AssessPersonSysNo | int | 是 | 评估人编码 |
| AssistSysNoList | array int | 否 | 所选生活辅具id |
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
| value | string | 否 | 值 |
| option | string | 否 | 选项 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | string | 是 | 组号 |
| GroupTitle | string | 是 | 组名 |
| QuestionList | array Question | 是 | 问题数组 |
| NOTEMSG | string | 是 | 生理功能与构造评估(左侧) |
| NOTEMSG2 | string | 是 | 辅具适配建议(左侧) |
| NOTEMSG_ACT | string | 是 | 生理功能与构造评估(右侧) |
| NOTEMSG_STR | string | 是 |  |
| NOTEMSG_LEN | string | 是 |  |
| NOTEMSG_CIR | string | 是 | 辅具适配建议(右侧) |
| FJList | array FJ | 是 | 推荐辅具列表（总） |
| FJGroupList | array FJGroup | 是 | 推荐辅具列表（总） |
| FJGroupLList | array FJGroup | 是 | 推荐辅具列表（左侧） |
| FJGroupRList | array FJGroup | 是 | 推荐辅具列表（右侧） |
| AssistantList | array Assistant | 是 | 推荐产品列表 |
| Side | string | 是 | 左侧、右侧 |
| Position | string | 是 | 断肢部位 |

FJ

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FJSysNo | int | 是 | 辅具id |
| ISO | string | 是 | ISO |
| FJName | string | 是 | 辅具名称 |
| IsMain | int | 是 | 1主件，0配件 |

Assistant

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantSysNo | int | 是 | 产品id |
| AssistantCode | string | 是 | 产品编号 |
| AssistantName | string | 是 | 产品名称 |
| BrandSysNo | int | 是 | 品牌id |
| BrandName | string | 是 | 品牌名称 |
| SupplierSysNo | int | 是 | 供应商id |
| SupplierName | string | 是 | 供应商名称 |

Question

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionNo | string | 是 | 问题编号 |
| Question | string | 是 | 问题内容 |
| QuestionType | int | 是 | 1单选，2多选，3填空 |
| Necessary | int | 是 | 1必须，0非必须 |
| Url | string | 否 | 问题资源 |
| AnswerList | array Answer | 是 | 答案数组 |

Answer

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AnswerNo | string | 是 | 答案编号 |
| Answer | string | 是 | 答案文本 |
| AnswerType | int | 是 | 1文本，2图片，3语音 |
| Url | array Answer | 是 | 资源链接 |