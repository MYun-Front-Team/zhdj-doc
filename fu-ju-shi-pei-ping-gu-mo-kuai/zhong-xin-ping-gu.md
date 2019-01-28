# 重新评估

_**【接口地址】**_

http://ip:port/FJAction/Adaption/ReAssess

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssessSysNo | int | 是 | 旧评估id |
| CancelReason | string | 是 | 作废理由 |
| PersonSysNo | int | 否 | 残疾人id |
| AssessPersonSysNo | int | 是 | 评估人id |

**如果AssessSysNo传0，则新建一个评估，且不需要取消理由**

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 新评估id |








