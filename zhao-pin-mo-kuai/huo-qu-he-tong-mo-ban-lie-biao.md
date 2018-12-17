#获取合同模板列表
##### _【功能说明】_ {#【功能说明】}

获取合同模板列表


_**【应用场景】**_

获取合同模板列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Contract/GetCertificateTemList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CertificateSysNo| int | 是 | 证书系统编码 |



#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CertificateTemSysNo| int | 是 | 证书模板系统编码 |
| SellerName| string| 是 | 签约主体 |
| PositionType| int | 是 | 合同类型 |
| TemplateName| string| 是 | 模板名称 |
| TemplateCode| string| 是 | 模板编码 |


