# 设置投票类型描述（Top图文招牌） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

投票模块-设置投票类型描述

_**【应用场景】**_

在某个投票类型列表页顶部，都有一个图文招牌描述。

注意：如果当前数据范围树枝叶不存在，则往上找通用的页字段配置。

_**【接口地址】**_

[http://ip:port/VoteAction/Vote/](http://ip:port/HMAction/River/AddRiver)SetVoteTypeDesc

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| VoteType | int | 是 | 类型 |
| VoteClassSysNo | int | 否 | 分类编码 |
| VoteDesc | string | 是 | 描述 |
| FilePath | string | 是 | 文件图片路径 |



