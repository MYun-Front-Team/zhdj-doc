# 下一组问题

_**【接口地址】**_

http://ip:port/FJAction/Adaption/NextQuestion

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionList | array object | 是 | 问题数组 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| QuestionSysNo | int | 是 | 问题id |
| AnswerSysNoList | array int | 是 | 答案数组 |


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
| Url | array Answer | 是 | 资源链接 |