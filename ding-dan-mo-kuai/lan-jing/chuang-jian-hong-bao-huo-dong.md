#创建红包活动

##### _【功能说明】_ {#【功能说明】}

创建红包活动

_**【应用场景】**_

创建红包活动

_**【接口地址】**_

http://ip:port/ActivityAction/RedEnvelope/AddRedEnvelope

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeTitle| string| 否 |红包标题|
| Amount| decimal| 否 |红包金额|
| StartTime| datetime| 否 |红包开始|
| EndTime| datetime| 否 |红包结束|
| StartCalculationTime| datetime| 否 |结算起始|
| EndCalculationTime| datetime| 否 |结算终止|




> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|


