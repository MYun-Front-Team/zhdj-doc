# 入住协议添加

##### _【功能说明】_ {#【功能说明】}
入住协议添加

_**【应用场景】**_

入住协议添加

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetSaleContractBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractSysNo | int | 是 | 协议系统编码|
| Limit | Limit | 是 | 显示限制|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractSysNo | int | 是 | 协议系统编码 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ContractName | string | 否 | 协议名称|
| ContractArea | decimal | 否 | 协议面积|
| ContractType | int | 否 | 协议类别|
| ContractClassSysNo | int | 否 | 协议分类（枚举） |
| StartDate | datetime | 否 | 开始时间 |
| EndDate | datetime | 否 | 结束时间 |
| Deposit | decimal | 否 | 押金 |
| Remark | decimal | 否 | 备注 |
| FilePathList | array string | 否 |照片 |
| FileUrlList | array string | 否 |照片 |
| ContractMonth | int | 否 |收费周期|
| ContractRooms | array[ContractRoom] | 否 |关联房间|
| SellerName | string | 否 |企业名称 |
| SellerMaster | string | 否 |企业法人 |
| SellerTel | string | 否 |企业法人联系电话 |
| ContractStatus | int | 是 | 协议状态（1正常，2即将过期，3已过期，4已中止，5已终止） |
| ObjectFileList| array File| 否（可选配置） | 附件 |



#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |
| FileUrl| string| 是 | 文件地址 |



###ContractRoom
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractRoomSysNo | int | 是 | 关联房间系统编码 |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
|ParkRoomType | int | 是 |房间类型|
| ParkRoomName| int | 否 | 房间名称|
| BuildingArea| decimal | 否 |总建筑面积|
| Rent| decimal | 否 |租金单价|
| ParkFloorName | string | 否 | 楼层名称 |
| BuildingName | string | 否 | 楼宇名称 |
| ParkName | string | 否 | 园区名称|


##Limit
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowContractRooms | int | 是 |是否显示关联房间 |




