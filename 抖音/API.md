
域名：https://www.douyin.com、https://www-hj.douyin.com



### 精选

https://www.douyin.com/jingxuan

method：GET

作用：设置cookie



### 搜索

https://www.douyin.com/aweme/v1/web/general/search/stream/

method：GET

重要参数：

-   keyword
-   offset

重要响应：

-   x-tt-logid



https://www.douyin.com/aweme/v1/web/general/search/single/

method：GET

重要参数：

-   keyword
-   offset：从10开始
-   search_id：x-tt-logid



https://www.douyin.com/aweme/v1/web/api/suggest_words/

method：GET

重要参数：

-   query



### 推荐

https://www.douyin.com/aweme/v2/web/module/feed/

method：POST

重要参数：

- count
- refresh_index
- pull_type：刷新时是1，其他为2
- awemePcRecRawData
- a_bogus

其他：

-   主页的推荐、视频的推荐，awemePcRecRawData参数不同



### 视频

详情：https://www.douyin.com/aweme/v1/web/aweme/detail/

method：GET

重要参数：

-   aweme_id
-   a_bogus



评论：https://www-hj.douyin.com/aweme/v1/web/comment/list/

method：GET

重要参数：

-   aweme_id
-   cursor：从0开始
-   a_bogus

其他：

-   无法查看全部



评论的评论：https://www-hj.douyin.com/aweme/v1/web/comment/list/reply/

method：GET

重要参数：

-   item_id
-   comment_id
-   cursor：从0开始
-   count：总数
-   a_bogus

其他：

-   不登录只能看到3条



弹幕：https://www.douyin.com/aweme/v1/web/danmaku/get_v2/

method：GET

重要参数：

-   item_id
-   start_time
-   end_time
-   duration



相关：https://www.douyin.com/aweme/v1/web/aweme/related/

method：GET

重要参数：

-   aweme_id
-   filterGids：已获取相关视频的id列表
-   refresh_index：从1开始，++
-   a_bogus



推荐：https://www.douyin.com/aweme/v2/web/module/feed/



### 用户

用户信息：https://www.douyin.com/aweme/v1/web/user/profile/other/

method：GET

重要参数：

-   sec_user_id



投稿：https://www.douyin.com/aweme/v1/web/aweme/post/

method：GET

重要参数：

-   sec_user_id
-   a_bogus

其他：

-   不登陆只能看到部分投稿





