# 取消抢班

##### _【功能说明】_ {#【功能说明】}

取消抢班

_**【应用场景】**_

取消抢班

注：人员如果为空，那么就用操作人的PersonSysNo；

_**【接口地址】**_

http://ip:port/RecruitAction/Recruit/SetRecruitPersonCancel

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| IsForce| int | 否 | 强制取消（0要是超出限制会报错提示，1超出限制也不报错） |
| CancelRemark| string| 是 |取消备注 |






#### _应答数据_ {#应答数据-}



