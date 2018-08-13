# 课程模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseSysNo | int | 是 | 课程系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| CourseClassSysNo | int | 否 | 分类编码（通用） |
| CourseClassName | string | 否 | 分类名称 |
| CourseName | Nvarchar\(50\) | 是 | 课程名称 |
| CourseContent | string | 否 | 课程描述 |
| CourseStatus | int | 是 | 课程状态：0新增，10上架，11下架 |
| Teacher | object | 否 | 教师（简版） |
| TagList | array object | 否 | 适用对象标签列表 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 附件路径列表 |
| FileUrlList | array string | 否 | 附件地址列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CourseActivityCount | int | 否 | 上课次数（来源于活动） |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| CourseClassSysNo | int | 否 | 分类编码（通用） |
| TagSysNo | int | 否 | 适用对象标签编码 |
| TeacherSysNo | int | 否 | 教师编码 |
| CourseStatusList |array int | 否 | 课程状态：0新增，10上架，11下架 |
| TeacherDepartmentSysNo| int | 否 | 教师部门|
|StartCourseActivityCount |int | 否 |开始上课次数|
|EndCourseActivityCount |int | 否 |终止上课次数|




> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowTeacher | int | 否 | 是否显示教师信息 |
| IsShowTagList | int | 否 | 是否显示适用对象标签列表 |
| IsShowFileUrlList | int | 否 | 是否显示附件 |
| IsShowCourseActivityCount | int | 否 | 是否显示上课次数 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



