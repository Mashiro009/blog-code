---
title: blog_bug
date: 2021-08-16 15:56:59
tags:
---

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