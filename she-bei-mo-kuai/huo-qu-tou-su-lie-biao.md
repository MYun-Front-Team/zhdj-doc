# 获取投诉列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmQuery/Equipment/GetComplainList](http://ip:port/EqmQuery/Equipment/GetComplainList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 运营商人员编码 |
| CustomerPersonSysNo | int | 否 | 消费者人员编码 |
| ComplainStatusList | array\[int\] | 否 | 1未处理，10已处理 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 消费者人员编码 |
| PersonName | string | 是 | 昵称 |
| AvatarUrl | string | 是 | 头像 |
| ContactPhone | string | 是 | 联系方式 |
| Reason | string | 是 | 申述理由 |
| FileUrlList | array\[string\] | 是 | 凭证列表 |
| EquipmentSysNo | int | 是 | 设备id |
| EquipmentName | string | 是 | 设备名称 |
| SN | string | 是 | SN号 |
| PCDCode | string | 是 | PCD编码 |
| PCDDescription | string | 是 | PCD描述 |
| Location | string | 是 | 具体位置 |
| EquipmentTypeSysNo | int | 是 | 设备类型编码 |
| EquipmentTypeName | string | 是 | 设备类型名称 |
| ProductGroupSysNo | int | 是 | 商品编码 |
| ProductGroupName | string | 是 | 商品名称 |
| OrderTime | datetime | 是 | 消费时间 |
| OrderAmount | decimal | 是 | 消费金额 |
| ComplainStatus | int | 是 | 1未处理，10已处理 |
| DealStatus | int | 是 | 1未处理，10同意，11拒绝 |
| DealPersonSysNo | int | 是 | 处理人编码 |
| DealPersonName | string | 是 | 处理人名称 |
| DealTime | datetime | 是 | 处理时间 |
| RefuseReason | string | 是 | 拒绝理由 |



