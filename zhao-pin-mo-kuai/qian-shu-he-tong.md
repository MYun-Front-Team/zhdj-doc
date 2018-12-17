# 签署合同
##### _【功能说明】_ {#【功能说明】}
签署合同


_**【应用场景】**_

签署合同


_**【接口地址】**_

http://ip:port/RecruitAction/Contract/SetContractStart

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractSysNo| int | 是 | 合同系统编码 |
| ContractStatus| int | 是 |合同状态（0待签 10已签 11拒签） |
| ContractStart| datetime| 否 |合同开始 |
| ContractEnd| datetime| 否 |合同结束 |
