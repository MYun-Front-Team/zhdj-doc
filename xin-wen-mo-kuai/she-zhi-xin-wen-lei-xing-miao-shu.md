# 设置新闻类型描述（Top图文招牌） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新闻模块-设置学习类型描述

_**【应用场景】**_

在某个新闻类型列表页顶部，都有一个图文招牌描述。

注意：如果当前数据范围树枝叶不存在，则往上找通用的页字段配置。

_**【接口地址】**_

[http://ip:port/NewsAction/News/](http://ip:port/HMAction/River/AddRiver)SetNewsTypeDesc

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶系统编码 |
| NewsType | int | 是 | 新闻类型 |
| NewsDesc | string | 是 | 新闻描述 |
| FilePath | string | 是 | 文件图片路径 |



