# 撤下 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新闻模块-撤下

_**【应用场景】**_

点击撤下后，不能在客户端展示。底层需通过InUserSysNo找到Person实体，冗余信息到撤下人相关字段中。

_**【接口地址】**_

[http://ip:port/NewsAction/News/](http://ip:port/HMAction/River/AddRiver)RemoveNews

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsSysNo | int | 是 | 系统编码 |



