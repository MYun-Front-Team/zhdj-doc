# 创建群 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

创建群

_**【应用场景】**_

创建群

注：群类型=1会话 表示的是单聊群。

注：创建人即是第一个群成员+创建人权限+管理员权限。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/Add](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)Group

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| GroupType | int | 是 | 群类型（枚举） |
| GroupClassSysNo | int | 否 | 群分类系统编码（会话类型时可为空）（类别树） |
| GroupID | string | 否 | 群ID |
| GroupName | string | 是 | 群名称 |
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

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |

####  {#应答数据-（巡河记录数组）}



