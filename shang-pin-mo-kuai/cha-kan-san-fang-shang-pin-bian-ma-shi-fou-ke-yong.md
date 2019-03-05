# 查看三方商品编码是否可用
##### _【功能说明】_ {#【功能说明】}

查看三方商品编码是否可用

_**【应用场景】**_

查看三方商品编码是否可用


_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/IfHaveSourceProductGroupCode


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码（新增时为0） |
| SourceProductGroupCode| string| 否 | 三方商品编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}
#### GroupBuy {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 是 | 是否存在|



