#创建请教单

##### _【功能说明】_ {#【功能说明】}

创建请教单

_**【应用场景】**_

创建请教单

_**【接口地址】**_

http://ip:port/EduAction/Leave/AddLeave

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo |int | 是 |学生班级DataRangeSysNo  |
| StudentSysNo | int | 是 |学生系统编码 |
| LeaveName| string| 是 | 请假名称|
| LeaveType| int| 是 | 请假类型|
| LeaveRemark| string| 是 | 申请理由|
| CreateTime| string| 是 | 创建时间|
| FilePathList | array string | 否 | 主图Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 主图Path列表（第一张为首图） |
| AuditPersonSysNo| int| 是 | 审核人编码|
| LeaveTimeList| array LeaveTime| 是 |请假时间|



###LeaveTime

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaveTimeStart| string| 是 | 请假开始|
| LeaveTimeEnd| string| 是 | 请假结束|

















