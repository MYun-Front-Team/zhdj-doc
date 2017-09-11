# 报名 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-报名

_**【应用场景】**_

活动报名。调用该接口的业务模块需提供该人的岗位，冗余到活动人员足迹表中。底层需通过InUserSysNo找到Person实体，冗余信息到人相关字段中。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/](http://ip:port/HMAction/River/AddRiver)SignUpActivity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |
| PersonPost | string | 否 | 人员岗位（业务模块中冗余） |
| PersonDepartment | string | 否 | 人员部门（业务模块中冗余） |
| Remark | string | 否 | 备注（累加格式：内容+时间+人） |



