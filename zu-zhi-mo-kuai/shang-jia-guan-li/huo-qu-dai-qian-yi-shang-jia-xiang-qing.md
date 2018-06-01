# 待迁移商家获取申请详情

##### _【功能说明】_ {#【功能说明】}

待迁移商家获取申请详情

_**【应用场景】**_

待迁移商家获取申请详情

注：

_**【接口地址】**_

http://ip:port/OrganizationQuery/Seller/GetTransfer

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 |旧人员系统编码 |

> #### _应答数据_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TransferSysNo | int | 是 | 迁移系统编码 |
| Remark | string | 否 | 迁移备注|
| NewPersonSysNo | int | 是 | 申请人系统编码 |
| NewPersonName | string | 是 | 申请人名字 |

