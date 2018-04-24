# 缴费

##### _【功能说明】_ {#【功能说明】}

缴费

_**【应用场景】**_

缴费

_**【接口地址】**_

http://ip:port/ParkAction/IndustryFee/PayFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeSysNo | int | 是 | 项目系统编码 |
| PayTime| datetime | 是 | 缴费时间|
| PayType| int | 是 | 缴费类型（端定义）|
| PaidFee| decimal | 是 | 实际缴费|
| PaidRemark| string | 是 | 缴费备注|
| PaidFilePathList | array string | 否 |凭证照片 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



