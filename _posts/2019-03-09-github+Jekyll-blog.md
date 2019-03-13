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

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

2.配置环境变量
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
3.安装jekyll

```
gem install jekyll bundler
```

4.验证结果

```
ruby -v
```

```
jekyll -h
```

```
puskar@puskar-hrms:~$ ruby -v
ruby 2.3.1p112 (2016-04-26) [x86_64-linux-gnu]
puskar@puskar-hrms:~$ jekyll -h
jekyll 3.8.5 -- Jekyll is a blog-aware, static site generator in Ruby
```

#### 2.建立博客

```
jekyll new myblog
```

```
cd myblog
```

```
bundle exec jekyll server
```

```
puskar@puskar-hrms:~/文档/github/jekyll-text-theme$ bundle exec jekyll server
Configuration file: /home/puskar/文档/github/jekyll-text-theme/_config.yml
            Source: /home/puskar/文档/github/jekyll-text-theme
       Destination: /home/puskar/文档/github/jekyll-text-theme/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
       Jekyll Feed: Generating feed for posts
                    done in 5.099 seconds.
 Auto-regeneration: enabled for '/home/puskar/文档/github/jekyll-text-theme'
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```


在浏览器中录入 [http://localhost:4000](http://localhost:4000)，查看结果

![实例3](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/3.png)


#### 3.使用模板

```
git clone https://github.com/Rekeryang/jekyll.github.io.git
```

**[Change Log](https://github.com/rekeryang/jekyll-text-theme/blob/master/CHANGELOG.md)** | **[中文](https://github.com/rekeryang/jekyll-text-theme/blob/master/README-zh.md)**
