# 设置会员卡状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置会员卡状态

_**【应用场景】**_

设置会员卡状态

_**【接口地址】**_

http://ip:port/WalletAction/MemberCard/SetMemberCardStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardSysNo | int | 否| 会员卡系统编码（二选一） |
| CardNo | string | 否 | 卡号（二选一） |
| CardStatus | int | 是 | 卡状态：0初始化，9已挂失，10已激活，11已删除 | 
| Remark| string | 是 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



