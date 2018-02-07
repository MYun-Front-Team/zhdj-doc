# 审核代理商 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

审核代理商

_**【应用场景】**_

审核代理商

_**【接口地址】**_

[http://ip:port/OrganizationAction/Agent/AuditA](http://ip:port/OrganizationAction/Customer/AddCustomer)gent

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AgentSysNo | int | 是 | 代理商系统编码 |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| AuditRemark | string | 否 | 备注，审核失败时必填 |

#### _应答数据 _ {#应答数据-}



