

**简要描述：** 

- 用户注册接口

**请求URL：** 
- ` http://xx.com/api/user/register `

**请求方式：**
- POST 

**是否需要登录**
- 否

**参数：** 

|参数名|必选|类型|说明|默认值|
|:----    |:---|:----- |-----    |---------|
|username |是  |string |用户名   |username |
|password |是  |string | 密码    |password |
|name     |否  |string | 昵称    |name	   |

**返回示例**

``` 
{
	"newslist": [
		{
			"id": 26754, 
			"author": "test33", 
			"pubDate": "2013-09-17 16:49:50.0", 
			"title": "asdfa", 
			"authorid": 253469, 
			"commentCount": 0, 
			"type": 4
		}
	], 
	"notice": {
		"replyCount": 0, 
		"msgCount": 0, 
		"fansCount": 0, 
		"referCount": 0
	}
}
```

**返回参数说明** 

|返回值字段	|类型及范围	|说明| 
|:-----  |:-----|-----											|
|groupid 			|int   		|用户组id，1：超级管理员；2：普通用户  			|
|catalog			|int		|[1-综合新闻|2-软件更新|3-所有]					|
|newsCount			|int		|新闻条数 |
|newsCount			|int		|新闻条数 |
|pageSize			|int		|每页条数 |
|news_list.id		|long		|新闻id |
|news_list.author	|string		|投递者名称 |
|news_list.title	|string		|新闻标题 |
|news_list.pubDate	|datetime	|发布日期 |
|news_list.authorid	|long		|投递者编号 |
|news_list.commentCount	|int	|评论数 |
|news_list.type		|long		|新闻类型 [0-链接新闻|1-软件推荐|2-讨论区帖子|3-博客|4-普通新闻|7-翻译文章] |
|notice.replyCount	|int		|未读评论数 |
|notice.msgCount	|int		|未读私信数 |
|notice.fansCount	|int		|新增粉丝数 |
|notice.referCount	|int		|未读@我数 |

**备注** 

- 更多返回错误代码请看首页的错误代码描述



