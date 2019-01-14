# 新增补贴比例

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddSubsidyType

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SubsidyTypeSysNo | int | 是 | 补贴比例id |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| SubsidyTypeName | string | 是 | 补贴人群类别 |
| Ratio | decimal | 是 | 比例 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 补贴比例id |





