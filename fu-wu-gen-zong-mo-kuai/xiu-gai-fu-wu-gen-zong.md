# 修改服务跟踪 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改服务跟踪

_**【应用场景】**_

修改服务跟踪

_**【接口地址】**_

[http://ip:port/TrackAction/](http://ip:port/HMAction/River/AddRiver)[T](http://ip:port/HMAction/River/AddRiver)rack[/E](http://ip:port/HMAction/River/AddRiver)ditTrack

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackSysNo | int | 是 | 系统编码 |
| TrackTitle | string | 是 | 标题 |
| TrackContent | string | 否（可选配置） | 内容 |
| TrackTime | string | 否（可选配置） | 时间 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| IsPublic | int | 否（可选配置） | 是否公开 |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |

#### _应答数据_ {#应答数据-}



