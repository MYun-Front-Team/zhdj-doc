# 设置模块积分配置 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置模块积分配置

_**【应用场景】**_

设置模块积分配置

_**【接口地址】**_

[http://ip:port/PointsAction/Points/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etPointsConfig

注：设置积分模块配置表的赠送默认配置项数据。

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsConfigSysNo | int | 是 | 积分配置系统编码 |
| PointsCycle | int | 是 | 赠送周期天数（用来判断一个周期内最多赠送次数，0无限） |
| MaxNum | int | 是 | 一个周期内最多赠送次数，0无限 |
| PointsValue | int | 否 | 默认值 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



