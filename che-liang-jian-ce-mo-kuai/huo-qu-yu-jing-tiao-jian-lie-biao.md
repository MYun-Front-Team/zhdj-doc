# 获取预警条件列表

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetRuleList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RuleSysNo | int | 是 | 规则id |
| RuleType | int | 是 | 1动力性（稳定车速），2经济性（实测值），3第一转向轮（侧滑量），4第二转向轮（侧滑量），5同一车辆两次检测间隔时间 |
| RuleName | string | 是 | 规则名称 |
| RuleValue | string | 是 | 规则值 |
| IsEnable | int | 是 | 0否1是 |
