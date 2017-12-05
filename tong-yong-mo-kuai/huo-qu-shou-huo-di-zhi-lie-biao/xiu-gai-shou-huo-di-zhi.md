# 修改收货地址 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改收货地址

_**【应用场景】**_

修改收货地址

注：通过SortNo=0即是默认地址，

_**【接口地址】**_

[http://ip:port/UMAction/Address/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditAddress

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddressSysNo | int | 是 | 系统编码 |
| AddressPerson | string | 是 | 联系人 |
| PersonGender | int | 否 | 性别：1男，2女 |
| PersonPhone | string | 是 | 电话 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| AddressDesc | string | 是 | 地址 |
| AddressHouseNumber | string | 否 | 门牌号 |
| IsDefault | int | 否 | 是否默认地址：0否，1是 |
| TagSysNoList | array int | 否 | 标签列表 |
| Longitude | decimal\(18,10\) | 否 | 经度 |
| Latitude | decimal\(18,10\) | 否 | 纬度 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



