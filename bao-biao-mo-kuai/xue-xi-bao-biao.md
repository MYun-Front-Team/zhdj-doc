# 新闻报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 8000100 | 学习报表按党组织 | 按DataRangeSysNo维度 |
| 8000101 | 学习报表按党组织 | 按学习类型维度 |




> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo| int | 否 | 党支部 |
| StudySysNo| int | 否 | 学习编码|
| StartTime| datetime| 是 | 开始时间 |
| EndTime| datetime| 是 | 结束时间 |
| StudyTypeList |array[int] | 是 | 类型（枚举） |



> #### 应答数据 （PageResponseBase）【8000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 党委支部名称|
| ChildrenCount| int| 是 | 孩子党委数|
| MomentPartyCount| int| 是 | 评论党员数|
| PartyCount| int| 是 | 党员数|
| Rate| decimal| 是 | 签到率|


> #### 应答数据 PageResponseStatistic 【8000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ChildrenCount| int| 是 | 孩子党委数|
| MomentPartyCount| int| 是 | 评论党员数|
| PartyCount| int| 是 | 党员数|
| Rate| decimal| 是 | 签到率|

> #### 应答数据 （PageResponseBase）【8000101】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudyType |int | 是 | 类型（枚举） |
| StudyTotalSecond | int | 否 | 学习总时长 |




> #### 应答数据 PageResponseStatistic 【8000101】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudyTotalSecond | int | 否 | 学习总时长 |
| PersonCount| int | 否 | 学习人数 |












