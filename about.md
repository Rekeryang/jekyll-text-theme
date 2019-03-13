---
layout: article
titles:
  en      : &EN       About
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  关于
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  關於
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       소개
  ko-KR   : *KO
key: page-about
---
* content
{:toc}

## 环境配置
参考[Jekyll官方文档](https://jekyllrb.com/docs/installation/)

>我用的是ubuntu18.04的一体机，如果是windows10系统的朋友建议安装ubuntu虚拟机，因为windows环境运行Ruby容易出现错误！

### 安装ruby

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

### 配置环境变量
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
### 安装jekyll

```
gem install jekyll bundler
```

### 验证结果

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

## 建立博客

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


## 使用模板

```
git clone https://github.com/Rekeryang/jekyll.github.io.git
```

### 代码高亮主题

TeXt 使用 [Tomorrow](https://github.com/chriskempson/tomorrow-theme) 作为它的代码高亮主题。

| `tomorrow` | `tomorrow-night` | `tomorrow-night-eighties` | `tomorrow-night-blue` | `tomorrow-night-bright` |
| --- |  --- | --- | --- |  --- |
| ![Tomorrow](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/highlight_tomorrow.png) | ![Tomorrow Night](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/highlight_tomorrow-night.png) | ![Tomorrow Night Eighties](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/highlight_tomorrow-night-eighties.png) | ![Tomorrow Night Blue](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/highlight_tomorrow-night-blue.png) | ![Tomorrow Night Bright](https://raw.githubusercontent.com/rekeryang/jekyll-text-theme/master/screenshots/highlight_tomorrow-night-bright.png) |

## 文档

### 开始

- [快速开始](https://rekeryang.com/jekyll-text-theme/docs/zh/quick-start)
- [从 1.x 升级到 2.x](https://rekeryang.com/jekyll-text-theme/docs/zh/update-from-1-to-2)

### 定制

- [配置](https://rekeryang.com/jekyll-text-theme/docs/zh/configuration)
- [导航栏](https://rekeryang.com/jekyll-text-theme/docs/zh/navigation)
- [布局](https://rekeryang.com/jekyll-text-theme/docs/zh/layouts)
- [Logo 和 Favicon](https://rekeryang.com/jekyll-text-theme/docs/zh/logo-and-favicon)
- [作者](https://rekeryang.com/jekyll-text-theme/docs/zh/authors)
- [国际化](https://rekeryang.com/jekyll-text-theme/docs/zh/i18n)

### 内容

- [撰写博客](https://rekeryang.com/jekyll-text-theme/docs/zh/writing-posts)
- [附加样式](https://rekeryang.com/jekyll-text-theme/docs/zh/additional-styles)
- [扩展](https://rekeryang.com/jekyll-text-theme/docs/zh/extensions)
- [Markdown 增强](https://rekeryang.com/jekyll-text-theme/docs/zh/markdown-enhancements)

## 示例

| Name | Description |
| --- | --- |
| [Home](https://rekeryang.com/jekyll-text-theme/test/) | 列表页 |
| [Archive](https://rekeryang.com/jekyll-text-theme/archive.html) | 归档页 |
| [Layout Examples](https://rekeryang.com/jekyll-text-theme/samples.html) | 各种布局示例 |

## 支持我

你的支持是我的动力。你可以通过以下方式支持我：

- 给该项目点赞 🌟
- 关注我的 Github


## 其他资源

在 *_includes/icon/social* 目录下有很多的社交产品图标，例如 Behance、Flickr、QQ、微信等，方便修改和使用。

## 协议

TeXt Theme 遵循 [MIT 协议](https://github.com/rekeryang/jekyll-text-theme/blob/master/LICENSE)。
