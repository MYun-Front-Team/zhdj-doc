#帮砍

帮砍

_**【应用场景】**_

帮砍

_**【接口地址】**_

http://ip:port/ShopAction/CutPirce/HelpCutPirce

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceSysNo| int | 是 | 砍价系统编码 |
| PersonSysNo| int | 否 | 人员系统编码 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### CutPirceResult 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceHelpSysNo| int | 是 | 砍价帮系统编码 |
| DelPirce| decimal| 否 |砍掉价格 |
| RewardAmont| decimal| 否 |奖励红包|




