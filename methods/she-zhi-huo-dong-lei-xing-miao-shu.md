# 设置活动类型描述（Top图文招牌） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-设置活动类型描述

_**【应用场景】**_

在某个活动类型列表页顶部，都有一个图文招牌描述。

注意：如果当前数据范围树枝叶不存在，则往上找通用的页字段配置。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/](http://ip:port/HMAction/River/AddRiver)SetActivityTypeDesc

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| ActivityType | int | 是 | 活动类型 |
| ActivityClassSysNo | int | 否 | 活动分类编码 |
| ActivityDesc | string | 是 | 活动描述 |
| FilePath | string | 是 | 文件图片路径 |



