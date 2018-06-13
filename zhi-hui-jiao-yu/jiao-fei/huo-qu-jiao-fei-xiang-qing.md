# 获取缴费详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取缴费详情

_**【应用场景】**_

获取缴费详情

_**【接口地址】**_

[http://ip:port/StudentFeeQuery/StudentFee/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)StudentFeeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费编码 |
| Limit | array | 否 | 限制条件 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| KeyWord | string | 否 | 关键字搜索（名称） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeBase | object | 是 | 基础字段 |
| StudentFeeStatistic | object | 否 | 统计字段 |



