
**简要描述：** 

- 用户注册接口

**请求URL：** 
- ` https://api.github.com/ `

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
	"current_user_url": "https://api.github.com/user",
	"current_user_authorizations_html_url": "https://github.com/settings/connections/applications{/client_id}",
	"authorizations_url": "https://api.github.com/authorizations",
	"code_search_url": "https://api.github.com/search/code?q={query}{&page,per_page,sort,order}",
	"emails_url": "https://api.github.com/user/emails",
	"emojis_url": "https://api.github.com/emojis",
	"events_url": "https://api.github.com/events",
	"feeds_url": "https://api.github.com/feeds",
	"followers_url": "https://api.github.com/user/followers",
	"following_url": "https://api.github.com/user/following{/target}",
	"gists_url": "https://api.github.com/gists{/gist_id}",
	"hub_url": "https://api.github.com/hub",
	"issue_search_url": "https://api.github.com/search/issues?q={query}{&page,per_page,sort,order}",
	"issues_url": "https://api.github.com/issues",
	"keys_url": "https://api.github.com/user/keys",
	"notifications_url": "https://api.github.com/notifications",
	"organization_repositories_url": "https://api.github.com/orgs/{org}/repos{?type,page,per_page,sort}",
	"organization_url": "https://api.github.com/orgs/{org}",
	"public_gists_url": "https://api.github.com/gists/public",
	"rate_limit_url": "https://api.github.com/rate_limit",
	"repository_url": "https://api.github.com/repos/{owner}/{repo}",
	"repository_search_url": "https://api.github.com/search/repositories?q={query}{&page,per_page,sort,order}",
	"current_user_repositories_url": "https://api.github.com/user/repos{?type,page,per_page,sort}",
	"starred_url": "https://api.github.com/user/starred{/owner}{/repo}",
	"starred_gists_url": "https://api.github.com/gists/starred",
	"team_url": "https://api.github.com/teams",
	"user_url": "https://api.github.com/users/{user}",
	"user_organizations_url": "https://api.github.com/user/orgs",
	"user_repositories_url": "https://api.github.com/users/{user}/repos{?type,page,per_page,sort}",
	"user_search_url": "https://api.github.com/search/users?q={query}{&page,per_page,sort,order}"
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



