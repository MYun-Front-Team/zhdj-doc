# 获取请假详情

##### _【功能说明】_ {#【功能说明】}

获取请假详情

_**【应用场景】**_

获取请假详情

_**【接口地址】**_

http://ip:port/EduQuery/Leave/GetLeaveBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaveSysNo| int| 是 | 请假单编码|


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaveSysNo| int| 是 | 请假单编码|
| LeaveName| string| 是 | 请假名称|
| LeaveType| int| 是 | 请假类型|
| AuditStatus| int| 是 | 审核状态（0待审核，10已审核，11教师驳回）|
| CancelStatus| int| 是 | 取消状态（0取消状态，10已取消）|
| LeaveRemark| string| 是 | 申请理由|
| CreateTime| string| 是 | 创建时间|
| FilePathList | array string | 否 | 主图Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 主图Path列表（第一张为首图） |
| AuditRecord| AuditRecord| 是 | 审核人|
| AuditPersonSysNo| int| 是 | 审核人编码|
| CreatePerson| Person| 是 | 创建人|
| CancelPerson| Person| 是 | 取消人|
| CancelTime| Person| 是 | 取消时间|
| LeaveTimeList| array LeaveTime| 是 |请假时间|
| StudentBase| StudentBase| 是 | 请假人|



###LeaveTime

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaveTimeStart| string| 是 | 请假开始|
| LeaveTimeEnd| string| 是 | 请假结束|