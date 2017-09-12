# 获取未读数量 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

朋友圈模块-获取未读数量

_**【应用场景】**_

朋友圈模块-获取未读数量，返回该树下UserSysNo匹配的Person的未读数量。

_**【接口地址】**_

[http://ip:port/MomentsQuery/Moments/GetUnReadedCount](http://ip:port/HMAction/River/AddRiver)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树系统编码 |

#### _响应数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UnReadedCount | int | 是 | 未读数量 |



