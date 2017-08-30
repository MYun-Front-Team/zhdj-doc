# 新增人员足迹 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增人员足迹

_**【应用场景】**_

新增人员足迹

_**【接口地址】**_

[http://ip:port/UMAction/Info/Add](http://ip:port/HMAction/River/AddRiver)InfoPersonFootPrint

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否 | 资讯系统编码 |
| SourceType | int | 是 | 足迹类型：0客户，1用户 |
| SourceSysNo | int | 是 | 对应系统编码 |
| Name | string | 否 | 姓名 |
| CellPhoneNo | string | 否 | 手机 |
| FootPrintType | int | 否 | 足迹类型:0普通，1报名，2分享，3点赞 |
| SignTime | string | 否 | 足迹时间 |
| SignPlace | string | 否 | 足迹地点（签到/活动地） |
| SignJson | string | 否 | 端自定义字段（原样返回） |
| Reason | string | 否 | 原因 |
| Remark | string | 否 | 备注 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FootPrintSysNo | int | 是 | 足迹系统编码 |



