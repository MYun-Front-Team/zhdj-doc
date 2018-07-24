#发起砍价

发起砍价

_**【应用场景】**_

发起砍价

_**【接口地址】**_

http://ip:port/ShopAction/CutPirce/AddCutPirce

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNo| int | 否 | 数据范围编码列表（店铺树） |
| PersonSysNo| int | 否 | 人员系统编码 |
| SkuSysNo| int | 否 |SKU系统编码 |
| InvitationCode| string | 否 |邀请码（填了就会强行改变之前的上级） |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### CutPirceResult 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceSysNo| int | 否 |系统编码 |
| DelPirce| decimal| 否 |砍掉价格 |
| NextDelPirce| decimal| 否 |下次砍掉价格 |
| IsFollow| int | 否 |是否关注 |




