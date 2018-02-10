# 修改商品推荐 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改商品推荐

_**【应用场景】**_

修改商品推荐

注：同一个数据节点，同一个行业，同一个区域，同一个时间段 商品去重复；

_**【接口地址】**_

[http://ip:port/ShopAction/Recommend/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)EditRecommend

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendSysNo | int | 是 | 系统编码 |
| CategorySysNo | int | 否 | 推荐行业系统编码 |
| AreaSysNo | int | 否 | 推荐区域系统编码 |
| PCDCode | string | 否 | 推荐区域PCDCode |
| PCDDesc | string | 否 | 推荐区域PCD描述 |
| RecommendStartTime | string | 是 | 启用开始时间 |
| RecommendEndTime | string | 是 | 启用结束时间 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



