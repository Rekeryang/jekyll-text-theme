---
title:  "github+jekyll搭建个人博客"
date:   2019-3-9 11:40:18 +0800

tags: jekyll github markdown 前端 blog RubyGems HTML CSS
author: rekeryang
---

* content
{:toc}

#### 1.环境配置
参考[Jekyll官方文档](https://jekyllrb.com/docs/installation/)

>我用的是ubuntu18.04的一体机，如果是windows10系统的朋友建议安装ubuntu虚拟机，因为windows环境运行Ruby容易出现错误！

1.安装ruby

`sudo apt-get install ruby-full build-essential zlib1g-dev`

2.配置环境变量
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
3.安装jekyll

`gem install jekyll bundler`

4.验证结果

`ruby -v`

`jekyll -h`

![实例1](/1.png ''实例1'')

#### 2.建立博客

`jekyll new myblog`

`cd myblog`

`jekyll s`

![实例2](/2.png ''实例2'')

在浏览器中录入 [http://localhost:4000](http://localhost:4000)，查看结果

![实例3](/3.png ''实例3')


#### 3.使用模板
