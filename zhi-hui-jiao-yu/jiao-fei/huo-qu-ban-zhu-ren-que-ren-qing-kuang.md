# 获取班主任确认情况

##### _【功能说明】_ {#【功能说明】}

获取班主任确认情况

_**【应用场景】**_

获取班主任确认情况

_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetConfirms

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费编码 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo|int| 是 | 班级范围编码 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| ConfirmStatus | int | 是 | 确认状态：0待确认，2部分确认，10已确认|
| ConfirmPerson | string | 是 | 确认人|
| ConfirmTime | string | 是 | 确认时间|





