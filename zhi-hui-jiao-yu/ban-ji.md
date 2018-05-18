# 班级模块-字段说明 {#新增河流}

> #### 班级基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 班级系统编码 |
| FatherDataRangeSysNo | int | 是 | 班级所属数据范围树父亲节点 |
| DataRangeSysNo | int | 是 | 班级所属数据范围树 |
| ~~GradeSysNo~~ | ~~int~~ | ~~是~~ | ~~年级系统编码~~ |
| ClassName | Nvarchar\(50\) | 是 | 班级名称 |
| ClassMotto | Nvarchar\(200\) | 否 | 班训 |
| HeadMasterWord | Nvarchar\(500\) | 否 | 班主任寄语 |
| ClassTeacherList | array object | 否 | 班主任列表（取默认值） |
| CollectivePhotoPathList | array string | 否 | 集体照Path文件列表 |
| CollectivePhotoUrlList | array string | 否 | 集体照Url文件列表 |
| ClassBannerPathList | array string | 否 | 班旗Path文件列表 |
| ClassBannerUrlList | array string | 否 | 班旗Url文件列表 |
|  |  |  |  |

> #### 班级统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassPersonCount | int | 否 | 班级人数 |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowClassTeacherList | int | 否 | 是否显示班级班主任列表（IsDefault=1\) |
| IsShowCollectivePhotoUrlList | int | 否 | 是否显示集体照图片 |
| IsShowClassBannerUrlList | int | 否 | 是否显示班旗图片 |
| IsShowClassPersonCount | int | 否 | 是否显示班级人数 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}



