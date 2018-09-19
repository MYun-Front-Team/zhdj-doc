# 修改 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改

_**【应用场景】**_

修改

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/E](http://ip:port/HMAction/River/AddRiver)ditActivity

注：活动已发布状态下不允许修改。

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 系统编码 |
| ActivityTitle | string | 是 | 标题 |
| ActivityContent | string | 是 | 内容 |
| MaxPersonNum | int | 是 | 人数上限 |
| ActivitySignUpStartTime | string | 是 | 报名开始时间 |
| ActivitySignUpEndTime | string | 是 | 报名结束时间 |
| ActivityStartTime | string | 是 | 活动开始时间 |
| ActivityEndTime | string | 是 | 活动结束时间 |
| ActivityPlace | string | 是 | 活动地点 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |
| HostPersonSysNo | int | 否 | 主持人编码 |
| HostPersonName | string | 否 | 主持人姓名 |
| PickRuleTemplateList | array object | 否 | 选人规则 |
| SponsorName | string | 否（可选配置） | 主办方 |
| CoSponsorName | string | 否（可选配置） | 协办方 |
| PlugInUnitList | array object | 否 | 插件列表（见活动新增接口） |
| ModuleRelationList | array object | 否（可选配置） | 关联模块列表（实体说明见活动） |
| CPSSysNoList | array\[int\] | 否 | CPS渠道列表 |



