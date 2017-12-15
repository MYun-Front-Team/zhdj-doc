# 商家模块-字段说明 {#新增河流}

> #### SellerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerSysNo | int | 是 | 商家系统编码 |
| SellerType | int | 否 | 商家类型（行业枚举） |
| SellerClassSysNo | int | 否 | 商家类别系统编码（类目树） |
| SellerClassName | string | 否 | 商家类别名称 |
| SellerLevelSysNo | int | 否 | 商家等级系统编码 |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| AuditRecord | object | 否 | 审核记录实体 |
| SellerStatus | int | 是 | 商家状态：0未缴费，1已缴费 |
| SellerName | string | 是 | 商家名称 |
| SellerShortName | string | 是 | 简称 |
| SellerTel | string | 否 | 商家联系电话 |
| SellerDesc | string | 否 | 商家描述 |
| SellerMaster | string | 否 | 商家负责人 |
| SellerPost | string | 否 | 商家负责人岗位 |
| SellerIDCard | string | 否 | 商家负责人身份证 |
| SellerGender | int | 否 | 商家负责人性别：1男，2女 |
| SellerPerson | string | 否 | 商家联系人 |
| SellerPersonPhone | string | 否 | 商家联系人电话 |
| SellerPersonPost | string | 否 | 商家联系人岗位 |
| PCDCode | string | 否 | 省市区代码 |
| PCDDescription | string | 否 | 省市区描述 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| IDCardPathList | array string | 否 | 身份证Path路径列表 |
| LicensePathList | array string | 否 | 营业执照Path路径列表 |
| IDCardUrlList | array string | 否 | 身份证Url路径列表 |
| LicenseUrlList | array string | 否 | 营业执照Url路径列表 |
| SellerLogoPathList | array string | 否 | 商家Logo路径列表 |
| SellerLogoUrlList | array string | 否 | 商家Logo的URL列表 |

> #### SellerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerSysNo | int | 否 | 商家系统编码 |
| AuditStatusList | Array\[int\] | 否 | 审核状态 |
| SellerStatusList | Array\[int\] | 否 | 商家状态 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IDCardUrlList | int | 否 | 是否显示身份证列表 |
| LicenseUrlList | int | 否 | 是否显示营业执照列表 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |


#### AuditRecord说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditRecordSysNo | int | 是 | 系统编码 |
| AuditDate | string | 是 | 审核时间 |
| AuditRemark | string | 否 | 审核备注 |
| AuditResult | int | 是 | 审核结果：10审核通过，11审核失败 |
| AuditPerson | object | 是 | 审核人实体（简） |



