# C端确认是否接受Offer
##### _【功能说明】_ {#【功能说明】}
C端确认是否接受Offer


_**【应用场景】**_

C端确认是否接受Offer


_**【接口地址】**_

http://ip:port/RecruitAction/Recruit/HandleOffer


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo |int | 否 | 招聘系统编码|
| HandleOfferStatus|int | 否 | Offer处理状态（0初始 1待处理 10通过，11不通过）|
| HandleOfferRmark|string | 否 | Offer处理备注|






