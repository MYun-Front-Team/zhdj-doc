# 获取抢工服务商列表
##### _【功能说明】_ {#【功能说明】}

获取抢工服务商列表


_**【应用场景】**_

获取抢工服务商列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Contract/GetRecruitServerList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionType| int | 否 |工作类型:0不限,1全职,2兼职 |



#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitServerSysNo| int | 是 | 服务商系统编码 |
| RecruitServerName| string| 是 |服务商名称 |

