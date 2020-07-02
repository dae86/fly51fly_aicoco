# fly51fly_aicoco
[“爱可可-爱生活”微博](https://weibo.com/fly51fly)内容按月分享
## fly51fly微博内容简介
微博账号@爱可可-爱生活是数据科学圈的网红，因每天分享大量精选的数据科学领域的学习资料而出名，深受粉丝关注和喜爱。该账号每天从早晨4-5点开始发微博，日均发布大几十条原创。目前爱可可老师已经发布几万条微博，移动端不利于查看，我希望能爬下来浏览。
## 分享内容
通过[weibo.cn](https://weibo.cn/)查找微博用户“爱可可-爱生活”，获取其userid
```
爱可可-爱生活  :1402400261
```
我们将利用微博爬虫项目[github.com/dataabc/weiboSpider](https://github.com/dataabc/weiboSpider)，按月爬取[“爱可可-爱生活”微博](https://weibo.com/fly51fly)，分享到github来。由于微博的反爬虫限制,不能一下全爬完,将会不定期更新。
## 爬虫配置
使用[github.com/dataabc/weiboSpider](https://github.com/dataabc/weiboSpider)
```
git clone https://github.com/dataabc/weiboSpider.git
cd weiboSpider
pip install -r requirements.txt
```
修改默认的config.json为以下:
```json
{
    "user_id_list": ["1402400261"],
    "filter": 1,
    "since_date": "2020-06-01",
	"end_date": "2020-6-30",
    "write_mode": ["csv", "txt"],
    "pic_download": 0,
    "video_download": 0,
    "cookie": "your cookie"
}
```
## 声明
我们不生产知识，我们只是知识的搬运工。
## 参考资料
- [微博账号@爱可可-爱生活](https://weibo.com/fly51fly)
- [github.com/dataabc/weiboSpider](https://github.com/dataabc/weiboSpider)
- [如何获取user_id](https://github.com/dataabc/weiboSpider/blob/master/docs/userid.md)
- [如何获取cookie](https://github.com/dataabc/weiboSpider#如何获取cookie)