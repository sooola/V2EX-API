# V2EX-API
==========
做项目时用到的API整理，欢迎提交补充。

# 目录

* [1.API](#1)
    * [1.1 每天热门帖子](#1.1)
    * [1.2 每天最新帖子](#1.2)
    * [1.3 帖子下的回复](#1.3)
    * [1.4 所有节点](#1.4)
    * [1.5 节点详情](#1.5)
    * [1.6 根据节点名获取所有帖子](#1.6)
    * [1.7 用户详情](#1.7)
    * [1.8 用户发的帖子](#1.8)

#### 域名
> 域名地址 ：https://www.v2ex.com/api/

<h1 id="1">1.API</h1>
<h2 id="1.1">1.1 每天热门帖子</h2>

#### 接口说明
> 获取每天热门帖子

#### 请求
> [GET] topics/hot.json

#### 例子
> https://www.v2ex.com/api/topics/hot.json

#### 返回结构
```
    {
        "id" : 316762,
        "title" : "讲真，你们为什么要买 macbook？",
        "url" : "http://www.v2ex.com/t/316762",
        "content" : "我不是程序员，我不是美工，我也不是什么艺术家，反正的我的职业和 iworks 没有半毛钱关系，我前年买了一台 macbook air ，港行 5900 人民币，买的唯一原因是为了体验一下装逼的感觉，现在已经习惯了 osx 的风格，我来谈谈优点：\u000D\u000A1 ，那个时候貌似 6000 的超级本选择面很窄\u000D\u000A2 ， macbook air 让我体验到了开盖即用，盒盖即待机的体验，习惯之后已经和手机和 pad 一样，没有关机的概念\u000D\u000A3 ，轻便，适合客厅沙发党\u000D\u000A4 ，待机时间长，再也不会可以用再拖一根尾巴\u000D\u000A5 ，鼠标扔了\u000D\u000A6 ，能屏幕镜像到 apple tv\u000D\u000A\u000D\u000A不过， air 这条产品线不知道将来是否还存在， Pro 太贵了，我也不需要，这个价格我更情愿买 windows 本，比如 surfacebook ，讲真，是不是 macbook 今后的发展方向只是专业人士？像我这种轻度用户是不是都应该用 ipad 去？但是 ipad 上如何下载种子后让迅雷下载？我在 mac 上操作的事情之一就是下载种子。。。。",
        "content_rendered" : "我不是程序员，我不是美工，我也不是什么艺术家，反正的我的职业和 iworks 没有半毛钱关系，我前年买了一台 macbook air ，港行 5900 人民币，买的唯一原因是为了体验一下装逼的感觉，现在已经习惯了 osx 的风格，我来谈谈优点：\u000D\u003Cbr /\u003E1 ，那个时候貌似 6000 的超级本选择面很窄\u000D\u003Cbr /\u003E2 ， macbook air 让我体验到了开盖即用，盒盖即待机的体验，习惯之后已经和手机和 pad 一样，没有关机的概念\u000D\u003Cbr /\u003E3 ，轻便，适合客厅沙发党\u000D\u003Cbr /\u003E4 ，待机时间长，再也不会可以用再拖一根尾巴\u000D\u003Cbr /\u003E5 ，鼠标扔了\u000D\u003Cbr /\u003E6 ，能屏幕镜像到 apple tv\u000D\u003Cbr /\u003E\u000D\u003Cbr /\u003E不过， air 这条产品线不知道将来是否还存在， Pro 太贵了，我也不需要，这个价格我更情愿买 windows 本，比如 surfacebook ，讲真，是不是 macbook 今后的发展方向只是专业人士？像我这种轻度用户是不是都应该用 ipad 去？但是 ipad 上如何下载种子后让迅雷下载？我在 mac 上操作的事情之一就是下载种子。。。。",
        "replies" : 119,
        "member" : {
            "id" : 102617,
            "username" : "cyberdaemon",
            "tagline" : "",
            "avatar_mini" : "//cdn.v2ex.co/avatar/2e1b/24a6/102617_mini.png?m=1444979047",
            "avatar_normal" : "//cdn.v2ex.co/avatar/2e1b/24a6/102617_normal.png?m=1444979047",
            "avatar_large" : "//cdn.v2ex.co/avatar/2e1b/24a6/102617_large.png?m=1444979047"
        },
        "node" : {
            "id" : 10,
            "name" : "mbp",
            "title" : "MacBook Pro",
            "title_alternative" : "MacBook Pro",
            "url" : "http://www.v2ex.com/go/mbp",
            "topics" : 2458,
            "avatar_mini" : "//cdn.v2ex.co/navatar/d3d9/4468/10_mini.png?m=1469591623",
            "avatar_normal" : "//cdn.v2ex.co/navatar/d3d9/4468/10_normal.png?m=1469591623",
            "avatar_large" : "//cdn.v2ex.co/navatar/d3d9/4468/10_large.png?m=1469591623"
        },
        "created" : 1477889507,
        "last_modified" : 1477889507,
        "last_touched" : 1477969664
    }
```
<h2 id="1.2">1.2 每天最新帖子</h2>

#### 接口说明
> 获取每天最新帖子

#### 请求
> [GET] topics/latest.json

#### 例子
> https://www.v2ex.com/api/topics/latest.json

#### 返回结构
>与热门帖子相同

<h2 id="1.3">1.3 帖子下的回复</h2>

#### 接口说明
> 获取帖子下的回复

#### 请求
> [GET] topics/hot.json

#### 参数列表
> body

|*Name*|*Type*|*Description*|*Required*|
|---|---|---|---|
|topic_id|int|帖子id|Y|

#### 例子
> https://www.v2ex.com/api/replies/show.json?topic_id=316762

#### 返回结构
```
{
        "id" : 3705429,
        "thanks" : 0,
        "content" : "装逼，保值，开发设计两不误…",
        "content_rendered" : "装逼，保值，开发设计两不误…",
        "member" : {
            "id" : 158373,
            "username" : "mzh",
            "tagline" : "None",
            "avatar_mini" : "//cdn.v2ex.co/gravatar/b7e702f599cb0b47fd10479f9d07339b?s=24&d=retro",
            "avatar_normal" : "//cdn.v2ex.co/gravatar/b7e702f599cb0b47fd10479f9d07339b?s=48&d=retro",
            "avatar_large" : "//cdn.v2ex.co/gravatar/b7e702f599cb0b47fd10479f9d07339b?s=73&d=retro"
        },
        "created" : 1477889683,
        "last_modified" : 1477889683
    }
```

<h2 id="1.4">1.4 所有节点</h2>

#### 接口说明
> 获取所有节点信息

#### 请求
> [GET] nodes/all.json

#### 参数列表
> body

|*Name*|*Type*|*Description*|*Required*|
|---|---|---|---|
|name|string|节点名字|Y|

#### 例子
> https://www.v2ex.com/api/nodes/all.json

#### 返回结构
```
 {
        "id" : 1,
        "name" : "babel",
        "url" : "http://www.v2ex.com/go/babel",
        "title" : "Project Babel",
        "title_alternative" : "Project Babel",
        "topics" : 1119,
         "header" : "Project Babel \u002D 帮助你在云平台上搭建自己的社区",
         "footer" : "V2EX 基于 Project Babel 驱动。Project Babel 是用 Python 语言写成的，运行于 Google App Engine 云计算平台上的社区软件。Project Babel 当前开发分支 2.5。最新版本可以从 \u003Ca href\u003D\u0022http://github.com/livid/v2ex\u0022 target\u003D\u0022_blank\u0022\u003EGitHub\u003C/a\u003E 获取。",
        "created" : 1272206882
    }
```
<h2 id="1.5">1.5 节点详情</h2>

#### 接口说明
> 获取节点详情

#### 请求
> [GET] nodes/show.json

#### 例子
> https://www.v2ex.com/api/nodes/all.json?name=python

#### 返回结构
>与所有节点返回结构相同

<h2 id="1.6">1.6 根据节点名获取所有帖子</h2>

#### 接口说明
> 根据节点名获取该节点下的所有帖子

#### 请求
> [GET] topics/show.json

#### 参数列表
> body

|*Name*|*Type*|*Description*|*Required*|
|---|---|---|---|
|node_name|string|节点名字|Y|

#### 例子
> https://www.v2ex.com/api/topics/show.json?node_name=python

#### 返回结构
>与每天热门帖子结构相同

<h2 id="1.7">1.7 用户详情</h2>

#### 接口说明
> 获取用户详情

#### 请求
> [GET] members/show.json

#### 参数列表
> body

|*Name*|*Type*|*Description*|*Required*|
|---|---|---|---|
|username|string|用户名|Y|

#### 例子
> https://www.v2ex.com/api/members/show.json?username=Livid

#### 返回结构
```
{
    "status" : "found",
    "id" : 1,
    "url" : "http://www.v2ex.com/member/Livid",
    "username" : "Livid",
    "website" : "",
    "twitter" : "",
    "psn" : "",
    "github" : "",
    "btc" : "",
    "location" : "91789",
    "tagline" : "Gravitated and spellbound",
    "bio" : "I’ve managed to make something I could call my own world, over time, little by little. And when I’m inside it, I feel kind of relieved.",
    "avatar_mini" : "//cdn.v2ex.co/avatar/c4ca/4238/1_mini.png?m=1466415272",
    "avatar_normal" : "//cdn.v2ex.co/avatar/c4ca/4238/1_normal.png?m=1466415272",
    "avatar_large" : "//cdn.v2ex.co/avatar/c4ca/4238/1_large.png?m=1466415272",
    "created" : 1272203146
}
```

<h2 id="1.8">1.8 用户发的帖子</h2>

#### 接口说明
> 获取用户发的帖子

#### 请求
> [GET] topics/show.json

#### 参数列表
> body

|*Name*|*Type*|*Description*|*Required*|
|---|---|---|---|
|username|string|用户名|Y|

#### 例子
> https://www.v2ex.com/api/topics/show.json?username=Livid

#### 返回结构
>与每天热门帖子结构相同
