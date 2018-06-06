# 获取项目统计

##### _【功能说明】_ {#【功能说明】}

获取项目统计

_**【应用场景】**_

获取项目统计

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryProject/GetParkProjectInfo



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProjectInfoTotal| ProjectInfoTotal| 是 | 汇总数量|
| ProjectInfoItems| array[ProjectInfoItem]| 是 | 明细数量|



> #### ProjectInfoTotal

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count| int | 是 | 协议数量|



> #### ProjectInfoItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count| int | 是 | 协议数量|
| ProjectStatus | int | 是 | 协议状态项目状态（0潜在，1洽谈，2入住，3长期） |





