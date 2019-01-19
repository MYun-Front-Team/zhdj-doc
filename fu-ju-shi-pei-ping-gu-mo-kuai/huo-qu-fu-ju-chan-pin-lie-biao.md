# 获取辅具产品列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetAssistantList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Keyword | string | 否 | 关键字 |
| CodeName | string | 否 | 编号名称 |
| AssistantType | string | 否 | 型号 |
| BrandSysNo | int | 否 | 品牌 |
| ABList | string | 否 | AB目录 |
| CategorySysNo | int | 是 | 分类id |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantSysNo | int | 是 | 产品id |
| AssistantCode | string | 是 | 产品编码 |
| AssistantName | string | 是 | 产品名称 |
| AssistantType | string | 是 | 型号 |
| SupplierSysNo | int | 是 | 供应商id |
| Supplier | string | 是 | 供应商 |
| BrandSysNo | int | 是 | 品牌id |
| Brand | string | 是 | 品牌 |
| CategorySysNo | int | 是 | 分类id |
| Category | string | 是 | 分类 |
| ABList | string | 是 | AB目录 |
| Unit | string | 是 | 单位 |
| AdaptionLimit | string | 是 | 适配上限 |
| UseableYear | string | 是 | 最低使用年限 |
| Range | string | 是 | 使用范围 |
| Description | string | 是 | 产品描述 |
| Urls | array string | 是 | 图片列表 |
| Price | decimal | 是 | 金额 |
| TrainningFee | decimal | 是 | 单节训练费 |
| Section | int | 是 | 训练节数 |
| ArchivesFee | decimal | 是 | 建档费 |
| Freight | decimal | 是 | 运费 |
| SetupFee | decimal | 是 | 安装费 |
| Property | string | 是 | 辅具属性 |
| Parameter | string | 是 | 主要参数 |
| Remark | string | 是 | 备注 |








