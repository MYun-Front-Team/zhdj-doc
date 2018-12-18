# 修改坑位 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改坑位

_**【应用场景】**_

修改坑位

注：同一个数据节点，同一个行业，同一个区域，同一个时间段不需要被投放多次；

非发布状态下可修改。

_**【接口地址】**_

[http://ip:port/ShopAction/Hollow/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditHollow

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |
| HollowType | int | 否 | 坑位类型：0链接，1商品，2店铺，3新闻,4录播,5消息,6活动，7商品推荐集合页 |
| LaunchCategorySysNo | int | 否 | 投放行业系统编码 |
| LaunchAreaSysNo | int | 否 | 投放区域系统编码 |
| LaunchPCDCode | string | 否 | 投放区域PCDCode |
| LaunchPCDDesc | string | 否 | 投放区域PCD描述 |
| HollowTitle | string | 否 | 坑位标题 |
| HollowContent | string | 否 | 坑位内容 |
| HollowStartTime | string | 否 | 启用开始时间 |
| HollowEndTime | string | 否 | 启用结束时间 |
| Remark | string | 否 | 备注 |
| HollowPathList | array string | 否 | 坑位主图path路径 |
| HollowObjectList | array object | 否 | 坑位中对象实体列表 |
| HollowLogoPathList | array string | 否 | 坑位LOGOpath路径 |
| HollowBackPathList | array string | 否 | 坑位背景path路径 |
| SortNo| int | 否 | 排序 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}



