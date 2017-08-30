# 新增业务积分配置 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

新增业务积分配置

_**【应用场景】**_

新增业务积分配置

_**【接口地址】**_

[http://ip:port/UMAction/Point/AddP](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ointConfig

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceType | int | 是 | 来源类型 |
| SourceSysNo | int | 是 | 来源编码 |
| SourceOperateType | int | 是 | 来源操作类型：0新增，1查看，2回复，3审核，4上传，5下载，6签到，10完结 |
| PointsValue | int | 是 | 积分值 |

> #### 应答数据 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointConfigSysNo | int | 是 | 系统编码 |



