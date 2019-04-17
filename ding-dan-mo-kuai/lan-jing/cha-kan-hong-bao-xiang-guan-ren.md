#查看红包相关人

##### _【功能说明】_ {#【功能说明】}

查看红包相关人

_**【应用场景】**_

查看红包相关人

_**【接口地址】**_

http://ip:port/ActivityQuery/RedEnvelope/GetRedEnvelopeItemList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|
| PersonName| string| 否 | 用户名称|
| StartAmount| decimal| 否 |起始金额|
| EndAmount| decimal| 否 |终止金额|
| StartPickTime| datetime| 否 |起始领取时间|
| EndPickTime| datetime| 否 |终止领取时间|


> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeItemSysNo| int| 否 | 红包明细编码|
| PersonName| string| 否 | 用户名称|
| PersonSysNo| int| 否 | 用户编码|
| Amount| decimal| 否 |红包金额|
| PickTime| datetime| 否 |领取时间|

