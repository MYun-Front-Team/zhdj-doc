# 获取资讯记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取资讯记录

_**【应用场景】**_

获取资讯记录

_**【接口地址】**_

[http://ip:port/UMQuery/Info/GetInfos](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否 | 资讯系统编码 |
| InfoStatus | int | 否 | 状态：0新增，10发布，11撤下 |
| InfoTitle | string | 否 | 资讯标题（主题） |
| Limit | array | 否 | 限制条件 |

> #### limit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowCover | int | 否 | 是否显示封面 |
| IsShowFileUrls | int | 否 | 是否显示文件图片列表 |
| IsShowFootPrintCount | int | 否 | 是否显示人员足迹总数 |
|  |  |  |  |

> #### _应答数据 （巡河记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |
| InfoTypeSysNo | int | 是 | 资讯模块类型系统编码（见概述） |
| InfoClassSysNo | int | 否 | 资讯分类编码 |
| InfoTitle | string | 是 | 资讯标题（主题） |
| InfoStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| PublishUserSysNo | int | 否 | 发布人编码 |
| PublishUserName | string | 否 | 发布人 |
| PublishTime | string | 否 | 发布时间 |
| RemoveUserSysNo | int | 否 | 撤下人编码 |
| RemoveUserName | string | 否 | 撤下人 |
| RemoveTime | string | 否 | 撤下时间 |
| MaxPersonNum | int | 否 | 人数上限 |
| InfoPlace | string | 否 | 活动地点 |
| InfoSignUpStartTime | string | 否 | 报名开始时间 |
| InfoSignUpEndTime | string | 否 | 报名结束时间 |
| InfoStartTime | string | 否 | 活动开始时间 |
| InfoEndTime | string | 否 | 活动结束时间 |
| FileUrls | array string | 否 | 文件图片列表 |
| FootPrintCountList | array object | 否 | 人员足迹总数列表 |

#### FootPrintCountList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| key | int | 是 | 人员足迹某状态key |
| value | int | 是 | 人员足迹该状态总数 |



