# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

投票模块-新增

_**【应用场景】**_

先根据页面，获取可选字段列表接口和积分配置列表接口，再新增。

注：对象与属性的属性的ModuleClassSysNo=0,ModuleSourceSysNo=VoteSysNo；

_**【接口地址】**_

[http://ip:port/VoteAction/Vote/Add](http://ip:port/HMAction/River/AddRiver)Vote

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| VoteType | int | 是 | 类型（枚举） |
| VoteClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| VoteTitle | string | 是 | 标题 |
| VoteContent | string | 是 | 内容 |
| VoteStartTime | string | 是 | 报名开始时间 |
| VoteEndTime | string | 是 | 报名结束时间 |
| Remark | string | 否（可选配置） | 备注 |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |
| SponsorName | string | 否（可选配置） | 主办方 |
| CoSponsorName | string | 否（可选配置） | 协办方 |
| Propertys | array object | 是 | 选项属性列表 |
| PickRuleTemplateList | array object | 否（可选配置） | 选人规则 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 系统编码 |



