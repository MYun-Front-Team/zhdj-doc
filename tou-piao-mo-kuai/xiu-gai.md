# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

投票模块-新增

_**【应用场景】**_

先根据页面，获取可选字段列表接口和积分配置列表接口，再新增。

_**【接口地址】**_

[http://ip:port/VoteAction/Vote/Add](http://ip:port/HMAction/River/AddRiver)Vote

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 系统编码 |
| VoteType | int | 否 | 类型（枚举） |
| VoteClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| VoteTitle | string | 否 | 标题 |
| VoteContent | string | 否 | 内容 |
| VoteStartTime | string | 否 | 报名开始时间 |
| VoteEndTime | string | 否 | 报名结束时间 |
| Remark | string | 否 | 备注 |
| PointsValues | array object | 否 | 积分赠送配置 |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| Propertys | array object | 否 | 选项属性列表 |
| PickRuleTemplateList | array object | 否 | 选人规则 |

#### _应答数据_ {#应答数据-}



