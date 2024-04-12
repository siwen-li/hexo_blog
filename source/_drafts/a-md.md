---
title: a.md
tags:
---

```
# 开启服务
hexo server

# 包括草稿
hexo s --draft

# 新建文章
hexo new a

# 新建草稿
hexo new draft b

# 发布草稿成为文章
hexo publish b

# 普通页面
hexo new page c

# 清空缓存
hexo cl
# 生成静态文章
hexo g

# 部署文章
hexo d
```

- [x] item 1
    - [x] item 1-1
    - [ ] item 1-2
    - [ ] item 1-3
    - [ ] item 1-4
- [ ] item 2
    - [ ] item 2-1
    - [ ] item 2-2
    - [ ] item 2-3
    - [ ] item 2-4

<iframe src="https://baidu.com" width="100%" height="500" name="topFrame" scrolling="yes"  noresize="noresize" frameborder="0" id="topFrame" loading="lazy"></iframe>


- 29^th^ => `29<sup>th</sup>`
- H~2~0 => `H<sub>2</sub>O`
- ==marked== => `<mark>inserted</mark>`
- ++inserted++ => `<ins>inserted</ins>`

!!! warning "aa"
    jing

!!! warning Hexo-admonition 插件使用示例
    这是基于 hexo-admonition 插件渲染的一条提示信息。类型为 note，并设置了自定义标题。
    提示内容开头留 4 个空格，可以有多行，最后用空行结束此标记。


!!! note "嵌套链接及引用块" 
    欢迎访问我的博客链接：[悟尘记](https://www.lixl.cn) 
    >这里嵌套一行引用信息。

!!! info a
    qywhiued

!!! missing b
    dshaiof