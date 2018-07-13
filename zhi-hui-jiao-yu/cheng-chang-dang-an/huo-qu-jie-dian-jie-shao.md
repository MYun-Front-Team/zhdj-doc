# 获取学期列表

##### _【功能说明】_ {#【功能说明】}

获取节点介绍

_**【应用场景】**_

获取节点介绍

_**【接口地址】**_

http://ip:port/EduQuery/Archives/GetEduDataRangeInf

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo| int| 是 | 节点编码 |
| Limit| int| 是 | 显示限制 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Introduce| string| 是 | 节点介绍 |
| VIPMessage| string| 是 | 院长寄语 |

> Limit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowIntroduce| string| 是 | 是否显示节点介绍 |
| VIPMessage| string| 是 | 是否显示院长寄语 |



















