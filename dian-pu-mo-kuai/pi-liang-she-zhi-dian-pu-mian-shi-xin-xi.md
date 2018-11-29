# 批量设置店铺面试信息

##### _【功能说明】_ {#【功能说明】}

批量设置店铺面试信息

_**【应用场景】**_

批量设置店铺面试信息

_**【接口地址】**_

http://ip:port/ShopAction/Shop/SetShopInterview

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ShopSysNoList |array[int] | 是 | 店铺系统编码 |
| InterviewBrand| string| 否 |面试品牌|
| InterviewPerson| string| 否 | 面试联系人 |
| InterviewPhone| string| 否 |面试联系人手机|
| InterviewPersonPost| string| 否 | 面试联系人职务 |
| InterviewAddress| string| 否 |面试联系人地址| 
| InterviewRemark| string| 否 | 面试备注 |
| ShopInterviewDateList | array ShopInterviewDate| 否 | 面试时间 |


#### ShopInterviewDate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate| datetime| 是 |开始面试时间（只有时分秒有效）|
| EndDate| datetime| 是 |结束面试时间（只有时分秒有效） |



#### _应答数据 _ {#应答数据-}



