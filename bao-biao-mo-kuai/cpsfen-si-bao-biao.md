#CPS粉丝报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 38000100 | 严选联盟CPS报表 | 严选联盟CPS报表 |


> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo|int | 是 |人员编码 |
| FansLeve| int| 否 | 1直接粉丝，2推荐粉丝|


> #### 应答数据 （PageResponseBase）【38000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机 |
| CreateTime| string | 否 | 创建时间 |
| CustomerLevelName| string | 否 | 客户等级 |
| CustomerLevelSysNo| string | 否 | 客户等级编码 |
| CustomerSonCount| int| 否 | 推荐孩子数 |
| FansLeve| int| 否 | 1直接粉丝，2推荐粉丝|

> #### 应答数据 PageResponseStatistic 【38000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerLevelName| string| 是 | 客户等级|
| FansCount| int| 是 | 数量|


> #### 应答数据 PageResponseStatistic 【38000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerLevelInfos| array CustomerLevelInfo| 否 | 各个客户等级人数 |



#### 应答数据 CustomerLevelInfo
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerLevelSysNo| string | 否 | 客户等级编码 |
| CustomerLevelName| string| 是 | 客户等级|
| FansCount| int| 是 | 数量|





