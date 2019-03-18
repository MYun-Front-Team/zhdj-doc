# 新增奖惩

_**【接口地址】**_

http://ip:port/PartyAction/Party/AddAwardPunish

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 干部id |
| GeneralType | int | 是 | 1奖励，2惩罚，3重大事项报告，4任免，5履职，6个人有关事项申报 |
| Year | string | 是 | 年度 |
| Level | string | 否 | 级别 |
| AwardType | string | 否 | 获奖类型 |
| PunishType | string | 否 | 处分 |
| Report | string | 否 | 重大事项报告 |
| FileList | array object | 否 | 附件列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileName | string | 是 | 附件名称 |
| FileUrl | string | 是 | 附件路径 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| APSysNo | int | 是 | 奖惩id |



