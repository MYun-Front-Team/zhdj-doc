#获取人员可领红包

##### _【功能说明】_ {#【功能说明】}

获取人员可领红包

_**【应用场景】**_

获取人员可领红包

_**【接口地址】**_

http://ip:port/ActivityQuery/RedEnvelope/GetCanPickRedEnvelopeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 否 | 人员编码|

> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|
| RedEnvelopeTitle| string| 否 |红包标题|
| Amount| decimal| 否 |红包金额|
| StartTime| datetime| 否 |红包开始|
| EndTime| datetime| 否 |红包结束|

