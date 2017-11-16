# 新增服务跟踪 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增服务跟踪

_**【应用场景】**_

先根据页面，获取可选字段列表接口和积分配置列表接口，再新增。

_**【接口地址】**_

[http://ip:port/TrackAction/](http://ip:port/HMAction/River/AddRiver)[T](http://ip:port/HMAction/River/AddRiver)rack[/Add](http://ip:port/HMAction/River/AddRiver)Track

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| PersonSysNo | int | 是 | 人员编码 |
| TrackType | int | 是 | 类型（枚举） |
| TrackClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| TrackTitle | string | 是 | 标题 |
| TrackContent | string | 否（可选配置） | 内容 |
| TrackTime | string | 否（可选配置） | 时间 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| IsPublic | int | 否（可选配置） | 是否公开 |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |
| ModuleRelationList | array object | 否（可选配置） | 关联模块列表（实体说明见活动） |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackSysNo | int | 是 | 系统编码 |



