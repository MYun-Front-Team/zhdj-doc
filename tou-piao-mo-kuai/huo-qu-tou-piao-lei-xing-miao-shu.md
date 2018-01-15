# 获取投票类型描述 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取投票类型描述

_**【应用场景】**_

获取投票类型描述

注：当DataRangeSysNo不存在描述记录时，往上找父级的类型描述。

_**【接口地址】**_

[http://ip:port/VoteQuery/Vote/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)VoteTypeDesc

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| VoteType | int | 是 | 类型（枚举） |
| VoteClassSysNo | int | 否 | 分类编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TopSysNo | int | 是 | 系统编码 |
| VoteDesc | string | 是 | 描述 |
| FileUrlList | array string | 是 | 文件图片URL列表 |



