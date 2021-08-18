---
title: blog_bug
date: 2021-08-16 15:56:59
tags: 
  - "hello"
  - "bugs"
---

# blog bug record

## 链接

[next 文档](https://theme-next.iissnan.com/getting-started.html)
we meet a bug when change the blog theme to next
Solution: [hexo使用theme出现问题](https://blog.csdn.net/qq_39898645/article/details/109181736)

[github建站系列(14) -- NexT 修改内容区域的宽度](https://kebingzao.com/2020/06/22/github-site-14/)
用的是 pisces 主题，所以直接在 Hexo/themes/next/source/css/_custom/custom.styl 补上内容
```
// Custom styles.
.header{
  width: 70%;
  +tablet() {
    width: 100%;
  }
  +mobile() {
    width: 100%;
  }
}
.container .main-inner {
  width: 70%;
  +tablet() {
    width: 100%;
  }
  +mobile() {
    width: 100%;
  }
}
.content-wrap {
  width: calc(100% - 260px);
  +tablet() {
    width: 100%;
  }
  +mobile() {
    width: 100%;
  }
}
```

[生成的blog的url含%20](https://github.com/iissnan/hexo-theme-next/issues/2233)
[解决NexT主题点击日志报错archives/%7C%7C%20archive](https://iqiqiya.com/posts/df32273d.html)
[Hexo博客NexT主题开启文章目录和调整样式](https://wugenqiang.github.io/articles/hexo-do-catalog.html)
[Hexo server报错TypeError: Cannot read property 'utcOffset' of null解决方法](https://www.cnblogs.com/mmzuo-798/p/10510225.html)

![png](/uploads/chicken.png)

## Hexo博客Next主题不显示作者名字和介绍
是因为其用的是主题配置文件里的author和description
```
要修改themes\next\_config.yml里面的author和description
```