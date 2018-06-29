# 活动报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 4000100 | 活动报表 | 按区域维度 |
| 4000101 | 活动报表 | 按时间维度 |
| 4000102 | 活动报表 | 按活动类型 |
| 4000103 | 活动报表 | 按活动汇总 |



> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityType|array[int] | 是 | 活动类型 |
| StartTime| datetime| 是 | 开始时间 |
| EndTime| datetime| 是 | 结束时间 |
| DataRangeSysNo| int | 是 | DataRangeSysNo |

> #### 应答数据 （PageResponseBase）【24000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 地区 |
| DataRangeSysNo| int | 是 | DataRangeSysNo |
| ActivityCount| int | 是 | 数量|


> #### 应答数据 PageResponseStatistic 【24000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityCount| int | 是 | 开展活动数量|
| ActivityPersonCount| int | 是 | 服务人次|


> #### 应答数据 （PageResponseBase）【24000101】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityStartTime| Datetime| 是 | 活动开始时间|
| Items| array[ActivityTimeItem] | 是 | 明细|

> #### 应答数据 ActivityTimeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityType| int| 是 | 活动类型 |
| ActivityCount| int | 是 | 数量|

> #### 应答数据 （PageResponseBase）【24000102】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityType| int| 是 | 活动类型|
| ActivityCount| int | 是 | 数量|





