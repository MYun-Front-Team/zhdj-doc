# 获取选人模板 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取选人模板

_**【应用场景】**_

获取选人模板

_**【接口地址】**_

[http://ip:port/PickQuery/Pick/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PickTemplate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TreeSysNo | int | 是 | 树系统编码（枚举） |
| DataRangeGradeType | int | 否 | 数据范围等级 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PickRuleTemplateList | array object | 是 | 选人规则（见模块说明） |



