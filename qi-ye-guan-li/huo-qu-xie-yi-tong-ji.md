# 入住协议添加

##### _【功能说明】_ {#【功能说明】}
入住协议添加

_**【应用场景】**_

入住协议添加

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetSaleContractInfo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractInfoTotal| ContractInfoTotal| 是 | 汇总数量|
| ContractInfoItems| array[ContractInfoItem]| 是 | 明细数量|



> #### ContractInfoTotal

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count| int | 是 | 协议数量|



> #### ContractInfoItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count| int | 是 | 协议数量|
| ContractStatus | int | 是 | 协议状态（1正常，2即将过期，3已过期，4已中止，5已终止） |









