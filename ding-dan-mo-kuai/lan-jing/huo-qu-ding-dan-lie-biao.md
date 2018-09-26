# CPS获取订单列表

##### _【功能说明】_ {#【功能说明】}

CPS获取订单列表

_**【应用场景】**_

CPS获取订单列表

_**【接口地址】**_

http://ip:port/OrderQuery/Order/GetLJOrderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string| 否 | 关键字 |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int |否 | 买家组织系统编码 |
| PersonSysNo | int | 否 | 买家人员系统编码 |


> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 否 |统计信息 |
| Details| array[Detail]| 否 |订单列表信息 |

#### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RewardMP| decimal| 否 | 总奖励魔力|
| WaitCodeCount| int| 否 | 待填订单号数量|
| WaitRewardCount| int| 否 | 等待奖励数量|




#### Detail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 买家人员系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| ReceiverName | string | 是 | 收货人 |
| ReceiverPhone | string | 是 | 收货电话 |
| ReceiverAddress | string | 是 | 收货地址 |
| PCDCode | string | 是 | 省市区 代码 |
| PCDDescription | string | 是 | 省市区 名称 |











