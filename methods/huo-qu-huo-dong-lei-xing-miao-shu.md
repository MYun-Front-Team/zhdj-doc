# 获取活动类型描述 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取活动类型描述

_**【应用场景】**_

获取活动类型描述。

注：当DataRangeSysNo不存在描述记录时，往上找父级的类型描述。

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityTypeDesc

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| ActivityType | int | 是 | 活动类型（枚举） |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TopSysNo | int | 是 | 系统编码 |
| ActivityDesc | string | 是 | 描述 |
| FileUrlList | array string | 是 | 文件图片URL列表 |



