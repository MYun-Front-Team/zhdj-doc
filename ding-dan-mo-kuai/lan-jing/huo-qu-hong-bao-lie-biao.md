# 获取红包列表

##### _【功能说明】_ {#【功能说明】}

获取红包列表

_**【应用场景】**_

获取红包列表

_**【接口地址】**_

[http://ip:port/ActivityQuery/RedEnvelope/GetRedEnvelopeList](http://ip:port/ActivityQuery/RedEnvelope/GetRedEnvelopeList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeStatus | int | 否 | 红包状态（0未开始 10进行中 11已结束） |
| StartTimeBegin | datetime | 否 | 起始开始时间 |
| StartTimeEnd | datetime | 否 | 截止开始时间 |
| EndTimeBegin | datetime | 否 | 起始终止时间 |
| EndTimeEnd | datetime | 否 | 截止终止时间 |
| StartAmount | decimal | 否 | 起始金额 |
| EndAmount | decimal | 否 | 终止金额 |
| RedEnvelopeType | int | 否 | 红包类型（1蓝晶红包，2魔力红包） |

> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RedEnvelopeSysNo | int | 否 | 红包编码 |
| RedEnvelopeTitle | string | 否 | 红包标题 |
| Amount | decimal | 否 | 红包金额 |
| StartTime | datetime | 否 | 红包开始 |
| EndTime | datetime | 否 | 红包结束 |
| StartCalculationTime | datetime | 否 | 结算起始 |
| EndCalculationTime | datetime | 否 | 结算终止 |
| RedEnvelopeStatus | int | 否 | 红包状态（0未开始 10进行中 11已结束） |
| PickAmount | decimal | 否 | 已领金额 |
| RestAmount | decimal | 否 | 剩余金额 |
| PersonCount | int | 否 | 红包人数 |
| PickPersonCount | int | 否 | 已领取人数 |
| Teams | array\[Team\] | 否 | 梯队 |
| RedEnvelopeType | int | 否 | 红包类型（1蓝晶红包，2魔力红包） |


#### Team

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeamName | string | 否 | 梯队名称 |
| TeamStartIndex | int | 否 | 梯队开始排名索引，（从0开始，0代表第一名） |
| TeamEndIndex | int | 否 | 梯队结束排名索引，（从0开始，0代表第一名） |
| SortNo | int | 否 | 排序（1第一梯队，2第二梯队） |
| Amount | decimal | 否 | 红包金额 |



