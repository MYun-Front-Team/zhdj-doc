# 获取预警条件详情

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetRuleBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RuleSysNo | int | 是 | 规则id |
| RuleType | int | 是 | 1动力性（稳定车速），2经济性（实测值），3第一转向轮（侧滑量），4第二转向轮（侧滑量），5同一车辆两次检测间隔时间 |
| RuleName | string | 是 | 规则名称 |
| IsEnable | int | 是 | 0否1是 |
| Relation | int | 是 | 1且，2或 |
| DetailList | array[object] | 是 | 明细列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DetailSysNo | int | 是 | 明细id |
| RuleSysNo | int | 是 | 规则id |
| DetailName | string | 是 | 条件名称 |
| Logic | int | 是 | 1=,2≠,3＜,4＞,5≤,6≥ |
| value | decimal(18,6) | 是 | 值 |
| Unit | string | 是 | 单位 |
