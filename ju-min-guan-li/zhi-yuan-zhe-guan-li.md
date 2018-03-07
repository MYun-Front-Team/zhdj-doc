# 志愿者管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| DataRangeName | string | 是 | 数据范围树名称 |
| VolunteerSysNo | int | 是 | 系统编码 |
| VolunteerStatus | int | 是 | 志愿者状态：1待审核，10审核通过，11审核失败 |
| OtherSpecialty | string | 否 | 其它特长与爱好 |
| VolunteerExperience | string | 否 | 义工或社工经历 |
| BuddhistExperience | string | 否 | 佛教经历 |
| Remark | string | 否 | 备注 |
| SpecialtyList | array object | 否 | 特长与爱好列表（分类） |
| Person | object | 否 | 人员实体 |
| Resident | object | 否 | 居民实体 |
| AuditRecordList | array object | 否 | 审核记录列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 否 | 数据范围树编码列表 |
| PersonSysNo | int | 否 | 人员系统编码 |
| VolunteerSysNo | int | 否 | 网格系统编码 |
| VolunteerStatus | int | 否 | 志愿者状态：1待审核，10审核通过，11审核失败 |
| SpecialtyClassSysNo | int | 否 | 特长与爱好编码（分类） |
| KeyWord | string | 否 | 关键字搜索（姓名，身份证，手机号） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPerson | int | 否 | 是否显示人员实体 |
| IsShowResident | int | 否 | 是否显示居民实体 |
| IsShowSpecialtyList | int | 否 | 是否显示特长与爱好列表 |
| IsShowAuditRecordList | int | 否 | 审核记录条数 |



