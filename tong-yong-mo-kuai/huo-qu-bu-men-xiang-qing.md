# 获取部门详情 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

获取部门详情

_**【应用场景】**_

获取部门详情

_**【接口地址】**_

[http://ip:port/UMQuery/Department/GetDepartmentBySysNo](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DepartmentSysNo | int | 是 | 部门系统编码 |

> #### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DepartmentSysNo | int | 是 | 部门系统编码 |
| DepartmentType | int | 是 | 部门类型 |
| DepartmentName | string | 是 | 部门名称 |
| Duty | string | 否 | 主要职责 |
| ContactName | string | 否 | 联系人 |
| ContactCellphone | string | 否 | 联系手机 |
| ContactTel | string | 否 | 联系电话 |
| Address | string | 否 | 地址 |
| PCDCode | string | 否 | PCDCode |
| PCDDescription | string | 否 | PCDDescription |
| DepartmentDesc | string | 否 | 部门描述 |
| Remark | string | 否 | 备注 |



