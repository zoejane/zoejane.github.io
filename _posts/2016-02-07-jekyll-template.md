---
layout: post
title:  "为Jekyll更换模板"
date:   2016-02-07 22:59:12 +0800
categories: Programiming
---

## 搜索模板
- Google搜索Jekyll Template
- 发现比较简洁的模板Hyde [Demo](http://hyde.getpoole.com/)  [代码下载](http://jekyllthemes.io/theme/8068127/hyde)

## 安装和使用模板
- 下载解压后复制到自己相应的GitHub repo，如zoejane.github.io
- 在terminal里运行jekyll serve

## 修复错误
### [错误1](https://teamtreehouse.com/community/jekyllpaginate-gem)
```
Deprecation: You appear to have pagination turned on, but you haven't included the `jekyll-paginate` gem. Ensure you have `gems: [jekyll-paginate]` in your configuration file.
```
- gem install jekyll-paginate  
- open _config.yml, add add the following line:
		```
		# Gems
		gems: [jekyll-paginate]
		```  
- run jekyll serve  

### [错误2](https://github.com/poole/poole/issues/99)
```
Since v3.0, permalinks for pages in subfolders must be relative to the site source directory, not the parent directory. Check http://jekyllrb.com/docs/upgrading/ for more info. 
```
- remove relative_permalinks: true from config.yml
