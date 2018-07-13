# 新增坑位 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增坑位

_**【应用场景】**_

新增坑位

注：同一个数据节点，同一个行业，同一个区域，同一个时间段不需要被投放多次；

_**【接口地址】**_

[http://ip:port/ShopAction/Hollow/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddHollow

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 投放组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（投放位置树） |
| HollowType | int | 是 | 坑位类型：0链接，1商品，2店铺，3新闻,4录播,5消息,6活动，7活动集合页 |
| LaunchCategorySysNo | int | 否 | 投放行业系统编码 |
| LaunchAreaSysNo | int | 否 | 投放区域系统编码 |
| LaunchPCDCode | string | 否 | 投放区域PCDCode |
| LaunchPCDDesc | string | 否 | 投放区域PCD描述 |
| HollowTitle | string | 是 | 坑位标题 |
| HollowContent | string | 否 | 坑位内容 |
| HollowStartTime | string | 是 | 启用开始时间 |
| HollowEndTime | string | 是 | 启用结束时间 |
| Remark | string | 否 | 备注 |
| HollowPathList | array string | 否 | 坑位主图path路径 |
| HollowObjectList | array object | 否 | 坑位中对象实体列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |



