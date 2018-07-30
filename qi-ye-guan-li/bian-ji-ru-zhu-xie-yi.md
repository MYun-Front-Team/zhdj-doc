# 入住协议添加

##### _【功能说明】_ {#【功能说明】}
入住协议添加

_**【应用场景】**_

入住协议添加

_**【接口地址】**_

http://ip:port/ParkAction/IndustrySale/EditSaleContract

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractSysNo | int | 是 | 协议系统编码 |
| OrganizationSysNo | int | 否 | 企业组织系统编码 |
| ContractName | string | 否 | 协议名称|
| ContractArea | decimal | 否 | 协议面积|
| ContractType | int | 否 | 协议类别|
| ContractClassSysNo | int | 否 | 协议分类（枚举） |
| StartDate | datetime | 否 | 开始时间 |
| EndDate | datetime | 否 | 结束时间 |
| Deposit | decimal | 否 | 押金 |
| Remark | decimal | 否 | 备注 |
| FilePathList | array string | 否 |照片 |
| ContractMonth | int | 否 |收费周期|
| ContractRooms | array[ContractRoom] | 否 |关联房间|
| ObjectFileList| array File| 否（可选配置） | 附件 |






###ContractRoom
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractRoomSysNo | int | 否 | （0新增，非0编辑） |
| ParkRoomSysNo | int | 是 | 房间系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



