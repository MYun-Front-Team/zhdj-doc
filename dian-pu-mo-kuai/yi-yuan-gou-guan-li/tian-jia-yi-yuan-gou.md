# 添加一元购

##### _【功能说明】_ {#【功能说明】}

添加一元购

_**【应用场景】**_

添加一元购

_**【接口地址】**_

http://ip:port/ShopAction/OneBuy/AddOneBuy


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo| int | 是 |平台编码 |
| DataRangeSysNo| int | 是 |店铺范围编码 |
| ProductGroupSysNoList|array[int] | 是 |款编码范围编码 |
| StartTime| datetime | 是 | 开始时间 |
| EndTime| int | 是 | 结束时间 |








> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |