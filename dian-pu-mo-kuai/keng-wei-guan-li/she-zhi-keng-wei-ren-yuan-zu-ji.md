# 设置坑位人员足迹 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置坑位人员足迹

_**【应用场景】**_

设置坑位人员足迹

注：收藏只允许一次；浏览目前可支持累计；（注意这里有人次）

_**【接口地址】**_

[http://ip:port/ShopAction/Video/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etHollowPersonStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |
| PersonStatus | int | 否 | 状态：0浏览，1收藏 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



