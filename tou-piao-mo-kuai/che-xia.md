# 撤下 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

投票模块-撤下

_**【应用场景】**_

投票点击撤下后，才能在客户端隐藏。底层需通过InUserSysNo找到Person实体，冗余信息到撤下人相关字段中。

_**【接口地址】**_

[http://ip:port/VoteAction/Vote/](http://ip:port/HMAction/River/AddRiver)RemoveVote

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 系统编码 |



