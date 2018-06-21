#获取我的砍价帮

获取我的砍价帮

_**【应用场景】**_

获取我的砍价帮

_**【接口地址】**_

http://ip:port/ShopQuery/CutPirce/GetMyCutPirceHelpList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceSysNo| int | 是 | 砍价系统编码 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### CutPirce {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceHelpSysNo| int | 是 | 砍价帮系统编码 |
| Person| Person | 是 | 砍价人 |
| DelPirce| decimal| 否 |砍掉价格 |
| CreateTime| string| 否 |时间 |
| Power| int| 否 |排行(0最给力，越大越不给力)|










