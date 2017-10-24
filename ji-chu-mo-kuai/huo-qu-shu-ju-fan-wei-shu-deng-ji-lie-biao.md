# 获取数据范围树等级列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取数据范围树等级列表

_**【应用场景】**_

获取数据范围树等级列表

_**【接口地址】**_

[http://ip:port/BasicQuery/Basic/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DataRangeGradeTypeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TreeSysNo | int | 是 | 树系统编码（枚举） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeGradeType | int | 是 | 等级类型 |
| DataRangeGradeName | string | 是 | 等级名称 |



