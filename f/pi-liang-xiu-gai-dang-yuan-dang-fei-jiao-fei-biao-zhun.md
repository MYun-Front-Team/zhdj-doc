# 批量修改党员党费缴费标准 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

批量修改党员党费缴费标准

_**【应用场景】**_

批量修改党员党费缴费标准

注：修改记录要保留日志。

_**【接口地址】**_

[http://ip:port/PartyAction/Party/E](http://ip:port/HMAction/River/AddRiver)ditDuesStandard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNoList | array int | 是 | 党员系统编码列表 |
| DuesStandard | decimal | 否 | 党费标准 |
| DuesDate | string | 否 | 党费交至年月 |



