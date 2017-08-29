## 本章节描述了所有接口通用内容，下面接口方法章节描述具体的数据内容，所有数据格式采用JSON格式 {#本章节描述了所有接口通用内容，下面接口方法章节描述具体的数据内容，所有数据格式采用json格式}

### 查询接口 {#查询接口}

> #### 请求数据 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 | 示例 |
| :--- | :--- | :--- | :--- | :--- |
| CompanyCode | Int | 是 | 项目号 | 14001 |
| UserSysNo | Int | 是 | 操作人编码 | 123456 |
| Extra | Object | 是 | 具体请求数据 | 参考具体接口 |
| Filters | Object Array | 否 | 过滤条件数组 | {DataType: '', Except: \[\]}\] |
| Sort | Object Array | 否 | 排序数组 | \[{SortName: 'CreateTime', SortType: 'Desc'}\] |
| PageIndex | Int | 否 | 分页页码\(1为第一页，0为全部\) | 1 |
| PageSize | Int | 否 | 分页页长 | 1 |

`注：Filters的Except有两种类型：Except和Include，分别表示排除和包含`

> #### 实例： {#实例：}

```
let
 param = {};
  param.CompanyCode = config.companyCode;
  param.UserSysNo = obj.UId || 
1
;

  param.Extra = {
    CustomerSysNo: obj.CId
  };

  param.Filters = [];
  param.Filters.push({
    DataType: 
'SaleTracking'
,
    Except: [
'CompanyCode'
, 
'CreateTime'
, 
'InUserSysNo'
, 
'InUser'
, 
'LastModifyTime'
,

'EditUserSysNo'
, 
'EditUser'
, 
'Status'
]
  });

  param.Sorts = [];
  param.Sorts.push({
    SortName: 
'CreateTime'
,
    SortType: 
'Desc'

  });
  param.PageIndex = 
1
;
  param.PageSize = 
9999
;
```

> #### 应答数据 {#应答数据}

| 变量名 | 类型 | 是否必须 | 描述 | 示例 |
| :--- | :--- | :--- | :--- | :--- |
| HasError | Boolean | 是 | 错误标示 | false |
| Fault | Object | 否 | 错误数据 | {ErrorCode: 0,ErrorDescription: ''} |
| Body | Object | 是 | 具体应答数据 | 参考具体接口 |

`注：Fault中ErrorCode为错误码，ErrorDescription为错误信息，当HasError为false时，分别是0和null`

> #### 实例： {#实例：}

```
  {

"Body"
: [{

"ProductGroupTagSysNo"
: 
1006922
,

"TagName"
: 
"新品"
,

"TagUrl"
: 
"#fd7140"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }, {

"ProductGroupTagSysNo"
: 
1006923
,

"TagName"
: 
"特卖"
,

"TagUrl"
: 
"#b98cef"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }, {

"ProductGroupTagSysNo"
: 
1006924
,

"TagName"
: 
"清仓"
,

"TagUrl"
: 
"#b3df64"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }, {

"ProductGroupTagSysNo"
: 
1006928
,

"TagName"
: 
"爆款"
,

"TagUrl"
: 
"#f2c138"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }, {

"ProductGroupTagSysNo"
: 
1006929
,

"TagName"
: 
"高端"
,

"TagUrl"
: 
"#70d3cc"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }, {

"ProductGroupTagSysNo"
: 
1006930
,

"TagName"
: 
"品牌"
,

"TagUrl"
: 
"#e1df3b"
,

"IsEnable"
: 
1
,

"Status"
: 
1

  }],

"Paging"
: {

"TotalCount"
: 
6
,

"PageSize"
: 
100
,

"CurrentPage"
: 
1

  },

"HasError"
: 
false
,

"Fault"
: {

"ErrorCode"
: 
0
,

"ErrorDescription"
: 
null

  }
}
```

### 操作接口 {#操作接口}

> #### 请求数据 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 | 示例 |
| :--- | :--- | :--- | :--- | :--- |
| CompanyCode | Int | 是 | 项目号 | 14001 |
| UserSysNo | Int | 是 | 操作人编码 | 123456 |
| Body | Object | 是 | 具体请求数据 | 参考具体接口 |

> #### 实例： {#实例：}

```
let
 param = {};
  param.CompanyCode = config.companyCode;
  param.UserSysNo = obj.UId || 
1
;

  param.Body = {
    RoleSysNo: obj.RoleId,
    RightSysNos: obj.Rights
  };
```

> #### 应答数据（参考查询类型） {#应答数据（参考查询类型）}



