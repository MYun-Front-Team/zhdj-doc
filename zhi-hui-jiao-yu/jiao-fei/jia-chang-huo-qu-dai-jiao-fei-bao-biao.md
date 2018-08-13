# 家长获取待缴费报表

##### _【功能说明】_ {#【功能说明】}

家长获取待缴费报表

_**【应用场景】**_

家长获取待缴费报表



_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetMySonStudentFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 是 | 汇总 |
| Items| List[Item]| 是 |明细 |

> #### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PayAbleAmount| decimal| 是 | 应缴金额 |




> #### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 学生人员编码 |
| StudentSysNo| int | 是 | 学生编码 |
| PersonName| string| 是 | 学生名称 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| PayAbleAmount| decimal| 是 | 应缴金额 |
| FilePathList|array string| 否 | 图片|
| FileUrlList|array string| 否 | 图片|














