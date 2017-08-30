# 新增党员转入转出记录 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增党员转入转出记录

_**【应用场景】**_

新增党员转入转出记录

_**【接口地址】**_

[http://ip:port/DMAction/Party/Add](http://ip:port/HMAction/River/AddRiver)PartyMemberMove

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 所属党员编码 |
| MoveInSysNo | int | 否（二选一必填） | 转入支部编码 |
| MoveOutSysNo | int | 否 | 转出支部编码 |
| MoveInTime | string | 否（二选一必填） | 转入时间 |
| MoveOutTime | string | 否 | 转出时间 |
| Remark | string | 否 | 备注 |
| FilePaths | array string | 否 | 文件路径列表 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MoveSysNo | int | 是 | 系统编码 |



