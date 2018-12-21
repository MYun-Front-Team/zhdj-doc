# 新闻报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 9000100 | 升级为社长的进度报表 | 升级为社长的进度报表 |
| 9000101 | 学习报表按党组织 | 按学习类型维度 |

> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 否 | 党支部 |


> #### 应答数据 PageResponseStatistic 【9000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FanLevel1| int| 是 |已购物并结算的一级理事|
| FanLevel2| int| 是 |已购物并结算的二级理事|
| FanLevel1Tar| int| 是 |一级理事(目标)|
| FanLevel2Tar| int| 是 |二级理事(目标)|


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













