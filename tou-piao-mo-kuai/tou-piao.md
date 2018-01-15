# 投票 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

投票

_**【应用场景】**_

投票

注：对象与属性值的属性的ModuleClassSysNo=1,ModuleSourceSysNo=PersonSysNo；

_**【接口地址】**_

[http://ip:port/VoteAction/Vote/](http://ip:port/HMAction/River/AddRiver)ConfirmVote

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| PersonStatus | int | 是 | 状态：10已投，11弃票 |
| Reason | string | 否 | 原因（状态=11时必填） |
| Remark | string | 否 | 备注 |
| Propertys | array object | 是 | 投票结果（状态=10时必填） |



