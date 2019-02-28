# 编辑预警条件

_**【接口地址】**_

http://ip:port/VDAction/Detect/EditRule

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RuleSysNo | int | 是 | 规则id |
| Relation | int | 是 | 1且，2或 |
| DetailList | array[object] | 是 | 明细列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DetailSysNo | int | 是 | 明细id |
| Logic | int | 是 | 1=,2≠,3＜,4＞,5≤,6≥ |
| value | decimal(18,6) | 是 | 值 |


> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


