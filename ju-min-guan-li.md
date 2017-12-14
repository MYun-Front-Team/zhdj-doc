# 居民模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSysNo | int | 是 | 系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| DataRangeName | string | 是 | 数据范围树枝叶名称 |
| LocalStatus | int | 否 | 人员类型：0未知，1本市人口、2流动人口、3境外人口 |
| MaritalStatus | int | 否 | 婚姻状态: 0未知，1未婚、2已婚、3丧偶、4离婚、5再婚、6其他 |
| AssistanceStatus | int | 否 | 社会救助状态：0否，1低保、2临保、3帮困 |
| PrivilegeStatus | int | 否 | 双拥优抚：0否，1病故属、2参战参试、3烈属、4军属、5伤残人员、6异地退休、7退伍安置、8立功受奖 |
| SpecialStatus | int | 否 | 特殊人群：0否，1残疾、2疾病防控人员、3刑满释放人员、4社区矫正人员、5涉毒人员、6精神病人员、7境外人员、8信访人员 |
| FollowStatus | int | 否 | 关注程度：0否，1关注 |
| ReligiousStatus | int | 否 | 宗教信仰：0无、1佛教、2伊斯兰教、10其他 |
| HealthyStatus | int | 否 | 健康状况：0亚健康、1健康、2非健康 |
| VolunteerStatus | int | 否 | 是否是志愿者：0否，1是 |
| PoliticalStatus | int | 否 | 政治面貌状态：0未知，1 中共党员,2 中共预备党员,3 共青团员,4 民革党员,5 民盟盟员,6 民建会员,7 民进会员,8 农工党党员,9 致公党党员,10 九三学社社员,11 台盟盟员,12 无党派人士,13 群众 |
| CarStatus | int | 否 | 是否有车辆：0否，1是 |
| DeathStatus | int | 否 | 是否死亡:0否，1是 |
| HouseholdRegisterAddress | string | 否 | 户籍地址 |
| HouseholdRegisterPolice | string | 否 | 户籍派出所 |
| FlowReason | string | 否 | 流动原因 |
| FlowDate | string | 否 | 流动时间 |
| FlowDataRangeSysNo | int | 否 | 流动来源数据范围系统编码 |
| FlowDataRangeName | string | 否 | 流动来源数据范围名称 |
| Person | object | 是 | 人员实体对象 |
| Remark | string | 否 | 备注 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| ResidentSysNo | int | 否 | 居民系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（标题/内容） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 2500101 | 居民模块 | 居民 |  | 新增页 |
| 2500102 |  | 居民 |  | 修改页 |
| 2500103 |  | 居民 |  | 详情页 |
| 2500104 |  | 居民 |  | 列表页 |



