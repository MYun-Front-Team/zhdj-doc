# 获取业务积分详情列表 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

获取业务积分详情列表

_**【应用场景】**_

获取业务积分详情列表

_**【接口地址】**_

[http://ip:port/UMQuery/Point/GetP](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ointsLogs

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsSysNo | int | 是 | 积分主键 |

#### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsLogSysNo | int | 是 | 日志系统编码 |
| ChangePointsValue | int | 是 | 积分变化值（区分正负） |
| NewPointsValue | int | 是 | 新积分值 |
| OldPointsValue | int | 是 | 旧积分值 |
| SourceTime | int | 是 | 有效期开始时间（小于当前时间即冻结） |
| SourceType | int | 是 | 来源类型 |
| SouceVoucherNo | string | 是 | 来源单据号 |
| Memo | string | 是 | 备注 |



