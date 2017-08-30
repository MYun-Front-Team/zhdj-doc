# 获取帮扶列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取帮扶列表

_**【应用场景】**_

获取帮扶列表

_**【接口地址】**_

[http://ip:port/DMQuery/Helper/G](http://ip:port/HMAction/River/AddRiver)etHelpers

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HelperSysNo | int | 否 | 帮扶记录系统编码 |
| HelperName | string | 否 | 帮扶姓名 |
| CellPhoneNo | string | 否 | 帮扶手机 |
| MemberName | string | 否 | 党员姓名 |
| MemberPhone | string | 否 | 党员手机 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HelperSysNo | int | 是 | 帮扶记录系统编码 |
| PartyMemberSysNo | int | 否 | 所属党员编码 |
| HelperName | string | 是 | 帮扶姓名 |
| CellPhoneNo | string | 否 | 手机 |
| HelperGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 出生年月 |
| ContractAddress | string | 否 | 联系地址 |
| HelperDesc | string | 否 | 帮扶说明 |
| HelperCycle | string | 否 | 帮扶周期 |
| Remark | string | 否 | 备注 |
| IsInCurrentParty | int | 否 | 是否在当前支部（查询人所在支部与查询结果党员所属支部比较） |



