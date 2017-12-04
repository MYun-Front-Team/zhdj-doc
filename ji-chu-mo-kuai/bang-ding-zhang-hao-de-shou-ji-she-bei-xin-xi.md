# 绑定账户的手机设备信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

绑定账号的手机设备信息

_**【应用场景】**_

绑定账号的手机设备信息

注：根据UserSysNo，更新账号的设备信息。

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etDeviceToken

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceType | int | 是 | 设备类型：1IOS，2安卓，3小米，4华为 |
| DeviceToken | string | 是 | 设备Token |

#### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceStatus | int | 是 | 设备状态：0原值不存在，1与原值相同，2与原值不同 |



