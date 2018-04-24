# 房间管理

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeSysNo | int | 是 | 费用系统编码 |
| FeeType | int | 是 | 费用类型 |
| FeeClassSysNo | int | 否 | 费用分类（枚举） |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| ParkSysNo| int | 否 | 园区编码|
| ParkName | string | 否 | 园区名称|
| SellerName | string | 否 |企业名称 |
| SellerSysNo | int | 否 |企业编码 |
| FeeItems | array FeeItem | 否 |费用详情 |
| TotalFee | decimal | 否 |总费用 |




> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### FeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeItemSysNo | int | 否 |费用明细编码 |
| FeeItemType| int | 否 |费用类型|
| Fee| decimal | 否 |费用|


> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





