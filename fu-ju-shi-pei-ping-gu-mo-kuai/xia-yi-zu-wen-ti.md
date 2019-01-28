# 下一组问题

_**【接口地址】**_

http://ip:port/FJAction/Adaption/NextQuestion

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int| 是 | 评估id |
| QuestionList | array object | 是 | 问题数组 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionSysNo | int | 是 | 问题id |
| AnswerSysNoList | array int | 是 | 选择题答案id数组 |
| AnswerList | array string | 否 | 填空题答案内容数组 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupTitle | string | 是 | 组名 |
| QuestionList | array Question | 是 | 问题数组 |
| NOTEMSG | string | 是 | 文本 |
| NOTEMSG2 | string | 是 | 文本 |
| NOTEMSG_ACT | string | 是 | 文本 |
| NOTEMSG_STR | string | 是 | 文本 |
| NOTEMSG_LEN | string | 是 | 文本 |
| NOTEMSG_CIR | string | 是 | 文本 |
| FJList | array FJ | 是 | 推荐辅具列表 |
| AssistantList | array Assistant | 是 | 推荐产品列表 |

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
| Url | array Answer | 是 | 资源链接 |