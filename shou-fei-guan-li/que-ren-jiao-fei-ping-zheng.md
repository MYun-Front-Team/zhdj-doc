# 确认缴费凭证

##### _【功能说明】_ {#【功能说明】}

确认缴费凭证

_**【应用场景】**_

确认缴费凭证

_**【接口地址】**_

http://ip:port/ParkAction/IndustryFee/AuditFeePayDetail

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeePayDetailSysNos |array int | 否 |支付凭着系统编码 |
| AuditStatus| int | 是 | 确认状态（10已确认，11作废）|
| PaidFilePathList | array string | 否 |凭证照片 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



