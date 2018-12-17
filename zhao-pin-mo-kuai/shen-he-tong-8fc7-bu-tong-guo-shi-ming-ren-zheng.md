# 审核通过/不通过实名认证

##### _【功能说明】_ {#【功能说明】}

审核通过/不通过实名认证

_**【应用场景】**_  
人员离职/在职

_**【接口地址】**_

http://ip:port/RecruitAction/Authentication/AuditAuthentication



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuthenticationSysNoList|array int | 是 | 系统编码 |
| PlatAuditStatus| int | 是 | 平台核验状态（10审核通过，0待审核，11审核不通过） |
| PlatAuditRemark| string  | 是 |审核备注|




