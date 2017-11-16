# 发布 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

发布

_**【应用场景】**_

点击发布后，才能在客户端展示。底层需通过InUserSysNo找到Person实体，冗余信息到发布人相关字段中。

积分备注：发布动作（枚举=15）预埋积分赠送逻辑。

_**【接口地址】**_

[http://ip:port/TrackAction/Track/](http://ip:port/HMAction/River/AddRiver)PublishTrack

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackSysNo | int | 是 | 系统编码 |



