# 新增商品图片 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增商品图片

_**【应用场景】**_

新增商品图片

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

注：该接口兼容款和sku的图片新增功能；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)ProductGroup[/A](http://ip:port/HMAction/River/AddRiver)ddProductImgList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~ProductGroupSysNo~~ | ~~int~~ | ~~是~~ | ~~款号系统编码~~ |
| ~~SkuSysNo~~ | ~~int~~ | ~~否~~ | ~~款规格系统编码~~ |
| ~~FileThumbnailPathList~~ | ~~array string~~ | ~~否~~ | ~~缩略图Path列表（第一张为首图）~~ |
| ~~FileMasterPathList~~ | ~~array string~~ | ~~否~~ | ~~主图Path列表（第一张为首图）~~ |

> #### 应答_数据_ {#请求数据}



