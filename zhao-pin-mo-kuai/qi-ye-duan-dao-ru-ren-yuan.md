# 企业端导入人员

##### _【功能说明】_ {#【功能说明】}

企业端导入人员

_**【应用场景】**_

企业端导入人员

_**【接口地址】**_

[http://ip:port/RecruitAction/Contract/ImportPersons]
(http://ip:port/RecruitAction/Contract/ImportPersons)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo| int| 是 | 组织编码 |
| Items| array[PersonItemAdd]| 是 | 人员明细 |



> #### _请求数据PersonItemAdd

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Index| int| 是 | 序号|
| RealName| string| 是 | 姓名 |
| CellPhoneNo| string| 是 | 手机号码|



#### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HasError| bool| 是 | 是否有错误|
| Errors| array[ImportPersonErrorItem]| 是 | 错误信息 |

#### _应答数据ImportPersonErrorItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Index| int| 是 | 序号|
| RealName| string| 是 | 姓名 |
| CellPhoneNo| string| 是 | 手机号码|
| ErrorMessage| string| 是 | 错误信息|

