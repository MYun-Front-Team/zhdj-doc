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

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeacherScore | decimal\(18,2\) | 否 | 评分 |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| ClassSysNo| int | 否 | 班级系统编码 |
| ClassTeacherType| int | 否 | 教师类型（类型： 1班主任，2副班主任，99教师） |



> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowTeacherScore | int | 否 | 是否显示评分 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



