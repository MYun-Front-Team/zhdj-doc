# 修改款（简版） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改款

_**【应用场景】**_

修改款

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/E](http://ip:port/HMAction/River/AddRiver)ditProductGroup2

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EditProductGroup | object | 是 | 修改款实体（见“修改款”） |
| SetProductImgList | object | 否 | 修改款图片（见“设置商品图片”） |
| ProductPrice | decimal\(18,2\) | 否 | 销售价格 |
| OnSaleStatus | int | 否 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |
| ProductOriginalPrice | decimal\(18,2\) | 否 | 原始价格 |
| ~~TagSysNoList~~ | ~~array int~~ | ~~否~~ | ~~标签系统编码列表~~ |

#### _应答数据 _ {#应答数据-}



