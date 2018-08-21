# 获取招聘领队报表

##### _【功能说明】_ {#【功能说明】}

获取招聘领队报表

_**【应用场景】**_

获取招聘领队报表

_**【接口地址】**_

http://ip:port/RecruitQuery/Recruit/GetLeaderPersonReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 查询条件 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaderPersonSysNo| int| 否 | 邀请人 |
| LeaderCellPhoneNo| string| 否 | 邀请人电话 |
| LeaderRealName| string| 否 | 邀请人姓名 |
| TotalCount| int| 否 | 总人数 |
| Items| array[Item]| 否 | 明细 |


> #### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count| int| 否 | 邀请人 |
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，20已上班，21放鸽子 |







