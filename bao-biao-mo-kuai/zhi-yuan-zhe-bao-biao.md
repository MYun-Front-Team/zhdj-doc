# 居民报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 25000100 | 志愿者报表 | 按区域维度 |
| 25000101 | 志愿者报表 | 按类型维度 |






> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 应答数据 （PageResponseBase）【25000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 地区 |
| DataRangeSysNo| int | 是 | DataRangeSysNo |
| VolunteerCount| int | 是 | 数量|

> #### 应答数据 （PageResponseBase）【25000101】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PoliticalStatus| int | 是 | 党派 |
| VolunteerCount| int | 是 | 数量|



