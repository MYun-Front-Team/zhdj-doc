# 审核\拒绝充值

##### _【功能说明】_ {#【功能说明】}

审核\拒绝充值

_**【应用场景】**_

审核\拒绝充值

_**【接口地址】**_

http://ip:port/RecruitAction/Wallet/SetRechargeStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RechargeSysNo | int | 是 | 充值编码 |
| RechargeStatus | int | 是 | 0待审核，10成功，11失败|
| Remark | string | 否 | 备注 |



