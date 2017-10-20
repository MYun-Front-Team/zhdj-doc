# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-新增

_**【应用场景】**_

先根据页面，获取可选字段列表接口和积分配置列表接口，再新增活动。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/Add](http://ip:port/HMAction/River/AddRiver)Activity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ActivityType | int | 是 | 类型（枚举） |
| ActivityClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
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
| ~~ActivityPersonConfig~~ | ~~object~~ | ~~否~~ | ~~默认参会人员配置~~ |
| PickRuleTemplateList | array object | 否（可选配置） | 选人规则 |
| SponsorName | string | 否（可选配置） | 主办方 |
| CoSponsorName | string | 否（可选配置） | 协办方 |

#### PointsValues说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsConfigSysNo | int | 是 | 积分配置系统编码 |
| PointsValue | int | 是 | 积分值 |

#### ~~ActivityPersonConfig说明~~ {#应答数据-}

| ~~变量名~~ | ~~类型~~ | ~~是否必须~~ | ~~描述~~ |
| :--- | :--- | :--- | :--- |
| ~~ModuleSysNo~~ | ~~int~~ | ~~是~~ | ~~模块编码（枚举）~~ |
| ~~ActivityPersonSourceType~~ | ~~int~~ | ~~是~~ | ~~参会人员类型：0Person，1模块自定义类型~~ |
| ~~ActivityPersonSourceSysNoList~~ | ~~array int~~ | ~~否~~ | ~~参会人员类型对应的编码列表（为空时，判断数据范围下的全部人员）~~ |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 系统编码 |



