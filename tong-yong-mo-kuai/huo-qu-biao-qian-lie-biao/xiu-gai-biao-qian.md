# 修改标签 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改标签

_**【应用场景】**_

修改标签

_**【接口地址】**_

[http://ip:port/UMAction/Tag/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditTag

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagSysNo | int | 是 | 系统编码 |
| TagName | string | 是 | 标签名称 |
| TagPathList | array string | 否 | 标签图片Path列表 |
| IconColor | string | 否 | 标签底色 |
| IsHidden | int | 否 | 是否对前台隐藏（1隐藏，0可见） |
| SortNo| int | 是 | 排序|
| PosterUrlList | array string | 否 | 海报URL列表 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}



