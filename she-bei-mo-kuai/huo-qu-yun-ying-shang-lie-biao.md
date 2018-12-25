# 获取运营商列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetSellerList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keywords | string | 否 | 关键字 |
| AuditStatusList | array int | 否 | 审核状态列表 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家编码 |
| OrganizationSysNo | int | 是 | 组织编码 |
| PersonSysNo | int | 是 | 人员编码 |
| SellerName | string | 是 | 运营商名称 |
| SellerPersonPhone | string | 是 | 手机号 |
| CreateTime | datetime | 是 | 注册时间 |
| EquipmentNum | int | 是 | 设备数 |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |



