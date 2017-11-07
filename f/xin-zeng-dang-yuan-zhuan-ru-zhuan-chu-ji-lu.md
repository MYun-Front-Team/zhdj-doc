# 新增党员转入转出记录 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增党员转入转出记录

_**【应用场景】**_

新增党员转入转出记录

_**【接口地址】**_

[http://ip:port/PartyAction/Party/Add](http://ip:port/HMAction/River/AddRiver)PartyMemberMove

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 否 | 所属党员编码 |
| RealName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机 |
| InnerPartyStatus | int | 是 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| MoveType | int | 是 | 类型：0转入，1转出 |
| MoveInSysNo | int | 是 | 转入支部编码 |
| MoveInName | string | 是 | 转入支部名称 |
| MoveOutSysNo | int | 是 | 转出支部编码 |
| MoveOutName | string | 是 | 转出支部名称 |
| MoveTime | string | 否 | 流转时间 |
| Remark | string | 否 | 备注 |
| FilePaths | array string | 否 | 文件路径列表 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MoveSysNo | int | 是 | 系统编码 |



