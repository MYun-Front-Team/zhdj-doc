# 根据项目标识符，获取全局变量列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据项目标识符，获取全局变量列表

_**【应用场景】**_

全局变量值如：OSS的上传参数、项目Logo等。

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)GlobalConfigList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| CanEdit| int | 是 | 可否允许后台编辑（0不允许，1允许）|
| KeyWord| string | 否 | 备注|


> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GlobalConfigSysNo | int | 是 | 系统编码 |
| ParamKey | string | 是 | key |
| ParamValue | string | 是 | value |
| Remark | string | 否 | 备注 |
| Describe| string | 是 | 详细描述|




