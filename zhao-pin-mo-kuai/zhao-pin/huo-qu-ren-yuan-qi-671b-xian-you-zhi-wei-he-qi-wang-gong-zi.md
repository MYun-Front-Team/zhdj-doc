# 获取人员期望/现有职位和期望工资

##### _【功能说明】_ {#【功能说明】}

获取人员期望/现有职位和期望工资

_**【应用场景】**_

获取人员期望/现有职位和期望工资

_**【接口地址】**_

http://ip:port/RecruitQuery/Recruit/GetPerson
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 |人员编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonPositions |array object | 是 | 基础字段 |
| PersonSalarys |array object | 否 | 统计字段 |

#### PersonSalary

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSalaryRelationSysNo | int | 否 | 系统编码 |
| SalaryType| int | 是| 薪资类型：1月，2天，3时|
| SalaryMax| decimal| 是 |最大值|
| SalaryMin| decimal| 是 |最小值|
| Remark| string | 否 |备注|



#### PersonPosition

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonPositionRelationSysNo | int | 是 | 系统编码 |
| PositionClassSysNo | int | 是 | 职位编码 |
| PositionName | int | 是 | 职位名称 |
| PersonPositionType| int | 是 | 类型：1期望，10做过 |


