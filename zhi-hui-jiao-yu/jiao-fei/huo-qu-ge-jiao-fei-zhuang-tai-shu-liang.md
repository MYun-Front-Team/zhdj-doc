# 获取各缴费状态数量

##### _【功能说明】_ {#【功能说明】}

获取各缴费状态数量

_**【应用场景】**_

获取各缴费状态数量

_**【接口地址】**_
http://ip:port/StudentFeeQuery/StudentFee/GetStudentFeeCountInfo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 见搜索条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditInfos| array[AuditInfo] | 是 | 审核状态 |
| PaidInfos| array[PaidInfo]| 否 | 缴费状态 |

#### AuditInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditStatus | int | 是 | 审核状态：0未提交，1审核中，10审核通过，11审核失败 |
| Count| int | 是 | 数量 |

#### PaidInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaidStatus | int | 是 | 缴费状态：0未开始缴费，1未下载，9缴费中，10缴费完成 |
| Count| int | 是 | 数量 |