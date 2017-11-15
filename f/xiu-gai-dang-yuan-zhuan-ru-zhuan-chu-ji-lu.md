# 获取党员转入转出记录列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取党员转入转出记录列表

_**【应用场景】**_

获取党员转入转出记录列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/G](http://ip:port/HMAction/River/AddRiver)etPartyMemberMoveList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 否 | 所属支部系统编码 |
| MoveSysNo | int | 否 | 系统编码 |
| MoveType | int | 否 | 类型：0转入，1转出，2流入，3流出 |
| PartyMemberSysNo | int | 否 | 所属党员编码 |
| ~~RealName~~ | ~~string~~ | ~~否~~ | ~~姓名~~ |
| ~~CellPhoneNo~~ | ~~string~~ | ~~否~~ | ~~手机~~ |
| KeyWord | string | 否 | 关键字搜索（姓名、手机号） |
| MoveStartTime | string | 否 | 转移开始时间 |
| MoveEndTime | string | 否 | 转移结束时间 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MoveSysNo | int | 是 | 系统编码 |
| PartyMemberSysNo | int | 否 | 所属党员编码 |
| RealName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机 |
| InnerPartyStatus | int | 是 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| MoveType | int | 是 | 类型：0转入，1转出，2流入，3流出 |
| MoveInSysNo | int | 是 | 转入支部编码 |
| MoveInName | string | 是 | 转入支部名称 |
| MoveOutSysNo | int | 是 | 转出支部编码 |
| MoveOutName | string | 是 | 转出支部名称 |
| MoveTime | string | 否 | 转移时间 |
| Remark | string | 否 | 备注 |
| FilePaths | array string | 否 | 文件路径列表 |



