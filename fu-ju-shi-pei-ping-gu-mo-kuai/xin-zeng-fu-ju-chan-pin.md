# 新增辅具产品

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddAssistant

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AssistantCode | string | 是 | 产品编码 |
| AssistantName | string | 是 | 产品名称 
| AssistantType | string | 是 | 型号 |
| SupplierSysNo | int | 是 | 供应商id |
| BrandSysNo | int | 否 | 品牌id |
| CategorySysNo | int | 是 | 分类id |
| ABList | string | 是 | AB目录 |
| Unit | string | 否 | 单位 |
| AdaptionLimit | string | 否 | 适配上限 |
| UseableYear | string | 否 | 最低使用年限 |
| Range | string | 否 | 使用范围 |
| Description | string | 否 | 产品描述 |
| Urls | array string | 否 | 图片列表 |
| Price | decimal | 是 | 金额 |
| TrainningFee | decimal | 是 | 单节训练费 |
| Section | int | 否 | 训练节数 |
| ArchivesFee | decimal | 否 | 建档费 |
| Freight | decimal | 否 | 运费 |
| SetupFee | decimal | 否 | 安装费 |
| Property | string | 否 | 辅具属性 |
| Parameter | string | 否 | 主要参数 |
| Remark | string | 否 | 备注 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 产品id |









