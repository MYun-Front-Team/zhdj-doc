# 新闻报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 7000100 | 新闻报表 | 按ClassSysNo维度 |


> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsType|array[int] | 是 | 新闻类型 |
| DataRangeSysNoList | array[int] | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |


> #### 应答数据 （PageResponseBase）【7000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsClassName| string | 是 | 类别名称|
| NewsClassSysNo| int | 是 | NewsClassSysNo|
| NewsCount| int | 是 | 数量|



