# 设置资讯状态 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置资讯状态

_**【应用场景】**_

发布或撤下资讯

_**【接口地址】**_

[http://ip:port/UMAction/Info/S](http://ip:port/HMAction/River/AddRiver)etInfoStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |
| InfoStatus | int | 是 | 状态：0新增，10发布，11撤下 |
| SourceOperateType | int | 否 | 来源操作类型：0新增，1查看，2回复，3审核，4上传，5下载，6签到，10完结（如传该参数，则判断是否需要赠送积分） |



