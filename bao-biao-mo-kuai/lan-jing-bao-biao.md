# 蓝晶报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 9000100 | 升级为社长的进度报表 | 升级为社长的进度报表 |
| 9000101 | 今日收益 | 今日收益 |
| 9000102 | 昨日收益 | 昨日收益 |
| 9000103 | 本月收益 | 本月收益 |
| 9000104 | 上月收益 | 上月收益 |
| 9000105 | 今年收益 | 今年收益 |
| 9000106 | 月账单 | 月账单 |
| 9000107 | 团队 | 团队 |
| 9000108 | 蓝晶排名 | 蓝晶排名  |
| 9000109 | 魔力排名 | 魔力排名  |
| 9000110|影响力排名 | 影响力排名  |
| 9000111|待唤醒好友 | 待唤醒好友  |
| 9000112|销售力排行 | 销售力排行 |
| 9000113|领导力排行 | 领导力排行 |
| 9000114|群主数据报表 | 群主数据报表 |
| 9000115|夺晶风云 | 夺晶风云|



> #### 请求数据（PageRequestData）\_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 |人员 |
| KeyWord | string | 否 | 关键字|
| PersonSysNoList |array[int] | 否 |人员列表 |
| StartTime| datetime| 否 | 开始时间|
| EndTime| datetime| 否 | 终止时间|




> #### 应答数据 PageResponseStatistic 【9000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FanLevel1 | int | 是 | 已购物并结算的一级理事 |
| FanLevel2 | int | 是 | 已购物并结算的二级理事 |
| FanLevel1Tar | int | 是 | 一级理事\(目标\) |
| FanLevel2Tar | int | 是 | 二级理事\(目标\) |

> #### 应答数据 PageResponseStatistic 【9000101/9000102】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MyMPPoints | decimal | 否 | 自购收益魔力 |
| MyAmount | decimal | 否 | 自购收益金额 |
| FanLevel1MPPoints | decimal | 否 | 一级理事魔力 |
| FanLevel1Amount | decimal | 否 | 一级理事金额 |
| FanLevel1Order | int | 否 | 一级理事订单 |
| FanLevel2MPPoints | decimal | 否 | 二级理事魔力 |
| FanLevel2Amount | decimal | 否 | 二级理事金额 |
| FanLevel2Order | int | 否 | 二级理事订单 |
| TeamMPPoints | decimal | 否 | 社长团队魔力 |
| TeamOrder | int | 否 | 社长团队订单 |
| TeamLevel1MPPoints | decimal | 否 | 一级社长团队魔力 |
| TeamLevel1Order | int | 否 | 一级社长团队订单 |
| TeamLevel2MPPoints | decimal | 否 | 二级社长团队魔力 |
| TeamLevel2Order | int | 否 | 二级社长团队订单 |
| TotalMPPoints | decimal | 否 | 总计魔力 |
| TotalAmount | decimal | 否 | 总计金额 |

> #### 应答数据 PageResponseStatistic 【9000103/9000104/9000105】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MyMPPoints | decimal | 否 | 自购预估收益魔力 |
| MyAmount | decimal | 否 | 自购预估收益金额 |
| MyOrder | int | 否 | 自购预估收益订单 |
| MySetMPPoints | decimal | 否 | 自购结算收益魔力 |
| MySetAmount | decimal | 否 | 自购结算收益金额 |
| MySetOrder | int | 否 | 自购结算收益订单 |
| FanLevel1MPPoints | decimal | 否 | 一级理事估收魔力 |
| FanLevel1Amount | decimal | 否 | 一级理事估收金额 |
| FanLevel1Order | int | 否 | 一级理事估收订单 |
| FanLevel1SetMPPoints | decimal | 否 | 一级理事结算魔力 |
| FanLevel1SetAmount | decimal | 否 | 一级理事结算金额 |
| FanLevel1SetOrder | int | 否 | 一级理事结算订单 |
| FanLevel2MPPoints | decimal | 否 | 二级理事估收魔力 |
| FanLevel2Amount | decimal | 否 | 二级理事估收金额 |
| FanLevel2Order | int | 否 | 二级理事估收订单 |
| FanLevel2SetMPPoints | decimal | 否 | 二级理事结算魔力 |
| FanLevel2SetAmount | decimal | 否 | 二级理事结算金额 |
| FanLevel2SetOrder | int | 否 | 二级理事结算订单 |
| TeamMPPoints | decimal | 否 | 社长团队预估收益魔力 |
| TeamOrder | int | 否 | 社长团队预估收益订单 |
| TeamSetMPPoints | decimal | 否 | 社长团队结算收益魔力 |
| TeamSetOrder | int | 否 | 社长团队结算收益订单 |
| TeamLevel1MPPoints | decimal | 否 | 一级社长团队预估魔力 |
| TeamLevel1Order | int | 否 | 一级社长团队预估订单 |
| TeamLevel1SetMPPoints | decimal | 否 | 一级社长团队结算魔力 |
| TeamLevel1SetOrder | int | 否 | 一级社长团队结算订单 |
| TeamLevel2MPPoints | decimal | 否 | 二级社长团队预估魔力 |
| TeamLevel2Order | int | 否 | 二级社长团队预估订单 |
| TeamLevel2SetMPPoints | decimal | 否 | 二级社长团队结算魔力 |
| TeamLevel2SetOrder | int | 否 | 二级社长团队结算订单 |
| TotalMPPoints | decimal | 否 | 总计预估魔力 |
| TotalAmount | decimal | 否 | 总计预估金额 |
| TotalSetMPPoints | decimal | 否 | 总计结算魔力 |
| TotalSetAmount | decimal | 否 | 总计结算金额 |


> #### 应答数据 （PageResponseBase）【9000106】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BillDate| datetime| 是 | 账单日|
| TotalMPPoints | decimal | 否 | 魔力 |
| TotalAmount | decimal | 否 | 金额 |

> #### 应答数据 （PageResponseBase）【9000107】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 否 | 昵称 |
| FileUrlList | array string | 否 | 头像图片列表 |
| CustomerLevelName | string | 否 | 客户等级 |
| TotalOrder | decimal | 否 | 已结算订单 |
| TotalMPPoints | decimal | 否 | 魔力 |
| TotalAmount | decimal | 否 | 金额 |
| SonCount| int| 否 | 共发展粉丝 |
| FrozenOrder| int| 否 | 冻结订单 |




> #### 应答数据 PageResponseStatistic 【9000107】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalFanCount| int| 否 | 总人数 |
| TeamFanCount| int| 否 | 下属团队人数|
| SonTeamFanCount| int| 否 |裂变团队人数|
| LowFanLevel1Count| int| 否 | 一级理事人数|
| LowFanLevel2Count| int| 否 | 二级理事人数|
| HigFanLevel1Count| int| 否 | 一级社长人数|
| HigFanLevel2Count| int| 否 | 二级社长人数|


> #### 应答数据 （PageResponseBase）【9000108，9000109，9000110，9000113，9000115】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IndexSort| int| 否 | 排序 |
| PersonName | string | 否 | 昵称 |
| IsEnable| int| 否 |启用状态 |
| FileUrlList | array string | 否 | 头像图片列表 |
| Value| decimal| 否 |值 |





> #### 应答数据 PageResponseStatistic 【9000108，9000109，9000110，9000113，9000115】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IndexSort| int| 否 | 排序 |
| PersonName | string | 否 | 昵称 |
| IsEnable| int| 否 |启用状态 |
| FileUrlList | array string | 否 | 头像图片列表 |
| IsEnable| int| 否 |启用状态 |
| Differ| decimal| 否 |和上一位差 |
| Value| decimal| 否 |值 |

> #### 应答数据 （PageResponseBase）【9000111】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 否 | 昵称 |
| FileUrlList | array string | 否 | 头像图片列表 |
| WeiXin | string | 否 | 微信|
| CellPhoneNo | string | 否 | 手机 |
| IsPublishCellPhone| int| 否 |是否公开手机号 |


> #### 应答数据 PageResponseStatistic 【9000111】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonCount| int| 否 | 待唤醒好友 |
| SleepPointMP | decimal | 否 | 待领取奖励|

> #### 应答数据 （PageResponseBase）【9000114】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 否 | 昵称 |
| NewSonCount| int| 是 | 新增直属理事数量|
| NewTeamCount| int| 是 | 新增团队人数数量|
| MySettlementOrderCount| int| 是 | 新增自购结算订单数|
| TeamSettlementOrderCount| int| 是 | 新增团队结算订单数|
| MyWaitOrderCount| int| 是 | 新增自购等待奖励订单数|
| TeamWaitOrderCount| int| 是 | 新增团队等待奖励订单数|
| MySettlementMPPoint| int| 是 | 自购结算魔力|
| TeamSettlementMPPoint| int| 是 | 团队结算魔力|
| MyFrozenMPPoint| int| 是 | 自购冻结魔力|
| TeamFrozenMPPoint| int| 是 | 团队冻结魔力|
| ChangeLanPoint| int| 是 |蓝晶数量|
| SettlementOrderAmount| decimal| 是 |结算订单金额|


