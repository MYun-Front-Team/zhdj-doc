# 修改代理商 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改代理商

_**【应用场景】**_

修改代理商

注：同一个代理区域只能有一个代理商；

_**【接口地址】**_

[http://ip:port/OrganizationAction/Agent/EditA](http://ip:port/OrganizationAction/Customer/AddCustomer)gent

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AgentSysNo | int | 是 | 代理商系统编码 |
| AgentType | int | 否 | 代理商类型（代理枚举） |
| AgentClassSysNo | int | 否 | 代理商类别系统编码（类目树） |
| AgentName | string | 否 | 代理商名称 |
| AgentShortName | string | 否 | 简称 |
| AgentTel | string | 否 | 代理商联系电话 |
| AgentDesc | string | 否 | 代理商描述 |
| AgentMaster | string | 否 | 代理商负责人 |
| AgentPost | string | 否 | 代理商负责人岗位 |
| AgentIDCard | string | 否 | 代理商负责人身份证 |
| AgentGender | int | 否 | 负责人性别：1男，2女 |
| AgentPerson | string | 否 | 代理商联系人 |
| AgentPersonPhone | string | 否 | 代理商联系人电话 |
| AgentPersonPost | string | 否 | 代理商联系人岗位 |
| PCDCode | string | 否 | 省市区代码 |
| PCDDescription | string | 否 | 省市区描述 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| IDCardPathList | array string | 否 | 身份证Path路径列表 |
| AgentLogoPathList | array string | 否 | 代理商Logo的Path路径列表 |
| AgentPCDCode | string | 否 | 代理区域Code |
| AgentPCDDescription | string | 否 | 代理区域描述 |

#### _应答数据 _ {#应答数据-}



