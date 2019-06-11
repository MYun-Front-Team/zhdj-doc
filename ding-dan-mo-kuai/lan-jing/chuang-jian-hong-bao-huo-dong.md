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
| StartTime| datetime| 否 |红包开始|
| EndTime| datetime| 否 |红包结束|
| StartCalculationTime| datetime| 否 |结算起始|
| EndCalculationTime| datetime| 否 |结算终止|
|Teams| array[Team]| 否 | 梯队|
| RedEnvelopeType | int | 否 | 红包类型（1蓝晶红包，2魔力红包） |


#### Team

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeamName| string| 否 | 梯队名称|
| TeamStartIndex| int| 否 | 梯队开始排名索引，（从0开始，0代表第一名）|
| TeamEndIndex| int| 否 | 梯队结束排名索引，（从0开始，0代表第一名）|
| SortNo| int| 否 | 排序（1第一梯队，2第二梯队）|
| Amount| decimal| 否 |红包金额|


> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo| int| 否 | 红包编码|


