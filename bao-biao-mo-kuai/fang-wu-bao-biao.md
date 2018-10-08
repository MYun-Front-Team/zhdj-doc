# 居民报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 25004100 | 居民报表按房屋| 居民报表按房屋 |




> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |




> #### 应答数据 （PageResponseBase）【25004100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 党委支部名称|
| ChildrenCount| int| 是 | 孩子党委数|
| MomentPartyCount| int| 是 | 评论党员数|
| PartyCount| int| 是 | 党员数|
| Rate| decimal| 是 | 签到率|


> #### 应答数据 PageResponseStatistic 【25004100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ChildrenCount| int| 是 | 孩子党委数|
| MomentPartyCount| int| 是 | 评论党员数|
| PartyCount| int| 是 | 党员数|
| Rate| decimal| 是 | 签到率|














