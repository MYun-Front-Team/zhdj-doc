# 教师模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeacherSysNo | int | 是 | 教师系统编码 |
| DataRangeSysNo | int | 是 | 学校所属数据范围树 |
| Person | object | 是 | 人员信息 |
| TeacherTitleSysNo | int | 否 | 教师职称系统编码（枚举） |
|  |  |  |  |
| TeacherContent | string | 否 | 描述 |
|  |  |  |  |
|  |  |  |  |
| MemberCards | array\[MemberCard\] | 是 | 教师卡包 |
| DataRanges | array\[DataRange\] | 是 | 教师班级权限 |
| UserSysNo | int | 是  |用户编码  |
| AdminStatus| int | 是  |用户状态  |
| Roles| array[Role] | 是  |角色  |




> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeacherScore | decimal\(18,2\) | 否 | 评分 |

#### MemberCard说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardSysNo | int | 是 | 会员卡系统编码 |
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡，3考勤卡,4一卡通，5教师考勤卡 |
| CardNo | string | 是 | 卡号 |

#### DataRange说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 系统编码 |
| DataRangeName | string | 是 | 权限树名称 |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表\(党建专用\) |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| ClassSysNo | int | 否 | 班级系统编码 |
| ClassTeacherType | int | 否 | 教师类型（类型： 1班主任，2副班主任，99教师） |
| EduDataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表\(教育专用\) |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowTeacherScore | int | 否 | 是否显示评分 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



