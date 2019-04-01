# 上一步

_**【接口地址】**_

http://ip:port/FJAction/Adaption/PrevQuestion

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int| 是 | 评估id |
| GroupSysNo | string | 否 | 组编号 |
| QuestionSysNoList | array string | 否 | 问题编号数组 |

注意：生活类评估不要传GroupSysNo 与 QuestionSysNoList 

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |