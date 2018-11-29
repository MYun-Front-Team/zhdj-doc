# 转链接口

转链接口

_**【应用场景】**_

转链接口

_**【接口地址】**_

http://ip:port/ProductAction/LJProductGroup/AddWantBuy

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|CPSProductID| string| 是 | 三方款主键|
| CPSCode|string| 是 | CPSCode|
| PersonSysNo|int| 是 | 人员编码|



> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WantBuySysNo| int | 是 | 想要系统编码|
| ProductGroupSysNo| int | 是 | 款系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
