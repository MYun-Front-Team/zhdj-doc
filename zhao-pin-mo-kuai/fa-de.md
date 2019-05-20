# 获取待签署协议列表

##### _【功能说明】_ {#【功能说明】}

获取待签署协议列表

_**【应用场景】**_

平台基础数据报表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Recruit/GetWaitSignContractList]
(http://ip:port/RecruitQuery/Wallet/GetWaitSignContractList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int| 是 | 人员编码 |


#### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractStatus| int | 是 | 协议签署状态，0未签署1无协议，10已签署11签署失败|
| WaitSignItems| array(WaitSignContract) | 是 |待签协议列表 |


> #### _应答数据WaitSignContract _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PesonSysNo| string | 是 | 人员编码|
| SellerSysNo| string | 是 | 客户编码|
| SellerName| datetime| 是 | 客户名称 |
| ContractStatus| int | 是 | 协议签署状态，0未签署10已签署11签署失败|






