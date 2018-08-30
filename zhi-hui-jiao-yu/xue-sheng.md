# 学生模块

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentSysNo | int | 是 |学生系统编码 |
| ClassSysNo | int | 是 | 学生班级编码 |
| ClassName| string| 是 | 学生班级 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| Person | object | 是 | 人员信息 |
| StudentNo| string| 是 | 学号 |
| UnionNo| string| 是 | 学籍号 |
| FreeType| int | 是 |1缴费用户、0未缴费用户、2公免用户 |
| MemberCards| array[MemberCard]| 是 |学生卡包 |


> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |

#### MemberCard说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberCardSysNo | int | 是 | 会员卡系统编码 |
| CardType | int | 是 | 会员卡类型：0会员卡，1礼品卡，2临时卡，3考勤卡,4一卡通 |
| CardNo | string | 是 | 卡号 |


> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| OrganizationFromSysNo| int | 是 | 微信登陆者组织 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| CellPhoneNo| string | 是 | 家长手机号 |


> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowMemberCards| int | 是 | 是否展示卡包 |


