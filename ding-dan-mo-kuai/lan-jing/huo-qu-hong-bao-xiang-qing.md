#获取红包详情

##### _【功能说明】_ {#【功能说明】}

获取红包详情

_**【应用场景】**_

获取红包详情

_**【接口地址】**_

http://ip:port/ActivityQuery/RedEnvelope/GetRedEnvelopeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|


> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|
| RedEnvelopeTitle| string| 否 |红包标题|
| Amount| decimal| 否 |红包金额|
| StartTime| datetime| 否 |红包开始|
| EndTime| datetime| 否 |红包结束|
| StartCalculationTime| datetime| 否 |结算起始|
| EndCalculationTime| datetime| 否 |结算终止|
| RedEnvelopeStatus| int| 否 | 红包状态（0未开始 10进行中 11已结束） |
| PickAmount| decimal| 否 | 已领金额|
| RestAmount| decimal| 否 | 剩余金额|
| PersonCount| int| 否 | 红包人数|
