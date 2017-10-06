# 修改群 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改群

_**【应用场景】**_

修改群

注：需判断操作人是否拥有设置的权限（管理员\创建人）

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| GroupName | string | 否 | 群名称 |
| GroupDesc | string | 否 | 群描述 |
| GroupAddress | string | 否 | 群地址 |
| PrivacyStatus | int |  | 隐私状态：0封闭（被搜索，不能看内容），1公开（被搜索，能看内容），2秘密（搜不到，不能看） |
| LifeCycleTime | string | 否 | 生命周期有效期 |
| IsNeedAudit | int | 否 | 是否需要审核（默认1需要审核） |
| Longitude | decimal\(18,10\) | 否 | 经度 |
| Latitude | decimal\(18,10\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 文件path路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



