7. 豆瓣爬虫

时间：2017年
https://github.com/fortyMiles/get_douban_comments
介绍：该项目为使用爬虫获得豆瓣电影评论的源代码，当年尚无相关法律规定。现在是否符合法律法规请大家自行查阅相关规定。



## Comment Spider 豆瓣电影评论爬虫程序

Author: Minchiuan(minchiuan.gao@gmail.com)

### Steps:

1. 因为豆瓣电影每个都有一个豆瓣自定义的movie-id, 所以首先用 BFS 搜索方式获得全网电影的movie-id；
2. 根据movie-id， 模拟手动浏览器行为获得comment页面；
3. 利用beautiful-soup进行解析。

### Requirements：

+ python >= 3.4
+ requests
+ beatifulsoup4


### How to Run:

1. 获取movie-id：

    ```bash
    $ python get_movie_id_bfs.py
    ```

2. 获得movie的评论;

    ```bash
    $ python douban_movie_comment_spider.py
    ```

### License:

MIT License
