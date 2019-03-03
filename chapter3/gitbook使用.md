# gitbook 使用

---

1. gitbook 初始化

在命令行输入命令
```
gitbook init
```
![init](/asserts/333.png)  
将会在当前目录下生成<font color=red>README.md</font>和<font color=red>SUMMARY.md</font>两个文件
>       
        README.md —— 书籍的介绍写在这个文件里
        SUMMARY.md —— 书籍的目录结构在这里配置

2. gitbook 发布

```
gitbook serve
```
默认将书籍发布在 [localhost:4000](localhost:4000)，可通过浏览器预览。也可以指定端口

```
gitbook serve --port 8080
```

3. gitbook 配置

  在书籍的顶级目录下创建 <font color=blue> book.json </font>，作为书籍的配置文件。
  ```
  {
    "title": "Blankj's Glory",
    "author": "Blankj",
    "description": "select * from learn",
    "language": "zh-hans",
    "gitbook": "3.2.3",
    "styles": {
        "website": "./styles/website.css"
    },
    "structure": {
        "readme": "README.md"
    },
    "links": {
        "sidebar": {
            "我的狗窝": "https://blankj.com"
        }
    },
    "plugins": [
        "-sharing",
        "splitter",
        "expandable-chapters-small",
        "anchors",

        "github",
        "github-buttons",
        "donate",
        "sharing-plus",
        "anchor-navigation-ex",
        "favicon"
    ],
    "pluginsConfig": {
        "github": {
            "url": "https://github.com/Blankj"
        },
        "github-buttons": {
            "buttons": [{
                "user": "Blankj",
                "repo": "glory",
                "type": "star",
                "size": "small",
                "count": true
                }
            ]
        },
        "donate": {
            "alipay": "./source/images/donate.png",
            "title": "",
            "button": "赞赏",
            "alipayText": " "
        },
        "sharing": {
            "douban": false,
            "facebook": false,
            "google": false,
            "hatenaBookmark": false,
            "instapaper": false,
            "line": false,
            "linkedin": false,
            "messenger": false,
            "pocket": false,
            "qq": false,
            "qzone": false,
            "stumbleupon": false,
            "twitter": false,
            "viber": false,
            "vk": false,
            "weibo": false,
            "whatsapp": false,
            "all": [
                "google", "facebook", "weibo", "twitter",
                "qq", "qzone", "linkedin", "pocket"
            ]
        },
        "anchor-navigation-ex": {
            "showLevel": false
        },
        "favicon":{
            "shortcut": "./source/images/favicon.jpg",
            "bookmark": "./source/images/favicon.jpg",
            "appleTouch": "./source/images/apple-touch-icon.jpg",
            "appleTouchMore": {
                "120x120": "./source/images/apple-touch-icon.jpg",
                "180x180": "./source/images/apple-touch-icon.jpg"
            }
        }
    }
}
```
  * title  
    标题

  * author  
    作者

  * language  
    语言，"zh-hans"表示中文, 其他还有 en, ar, bn, cs, de, en, es, fa, fi, fr, he, it, ja, ko, no, pl, pt, ro, ru, sv, uk, vi, zh-tw

  * styles  
    自定义页面样式

  * structure
    指定 Readme、Summary、Glossary 和 Languages 对应的文件名

  * links  
    在左侧导航栏添加链接信息

  * plugins  
    配置使用的插件

  * pluginsConfig  
    配置插件的属性

4. git 常用插件

  * expandable-chapters-small  
    使左侧章节可折叠
  * Disqus
    添加Disqus评论
  * popup
    弹出大图
