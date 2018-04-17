# 移动商品到分组

##### _【功能说明】_ {#【功能说明】}

移动商品到分组


_**【应用场景】**_

删除商品分组


_**【接口地址】**_
http://ip:port/ProductAction/ProductGroup/RemoveProductToGroup



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 否 | 商品组系统编码（0为搞到未分组里） |
| OrganizationSysNo| int | 是 | 组织编码 |
| DataRangeSysNo | int | 否 | 数据范围枝叶编码 |
| ProductGroupSysNoList | array[int]| 是  | 商品系统编码|



