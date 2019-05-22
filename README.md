# Browse Manager

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE) [![GitHub stars](https://img.shields.io/github/stars/ZDL-Git/browse-manager.svg)](https://github.com/ZDL-Git/browse-manager/stargazers)

### 项目说明

Chrome扩展：实现网址/域名拉黑，访问次数统计，自动收藏。

项目主页：https://github.com/ZDL-Git/browse-manager

### Idea来源

在搜索资源，或者查找解决棘手bug的方法的时候，会经历很长时间来回不断地翻阅一些网站，有的问题甚至半年后还需要重新来过。那些曾经访问过且证明没有任何意义的网页，会因为一个“优秀的”标题而导致再次浪费我们的时间。所以为什么我们不能统计它们，拉黑它们呢？

### 当前功能

<img src="https://github.com/ZDL-Git/resources-store/blob/master/images/popup.jpg?raw=true" width="40%"/>

* 拉黑地址或域名：黑名单，在页面右键-Browse Manager-URL不再访问(黑名单)/Domain不再访问(黑名单)；
* 统计访问次数：统计除白名单外每个网页已经访问过的次数，在图标上显示；
* 白名单：为了避免无用的统计，提供了白名单。页面右键将地址或域名加入白名单，不再统计、不再显示访问次数。"chrome:"/"www.baidu.com"/"www.google.com"开头的网页默认在白名单；
* 自动收藏：在管理界面（单击图标）设置自动收藏次数及收藏夹名称，当达到访问次数后网页会被自动收藏到指定收藏夹中，图标上的数字会变为红色。前期手动收藏过的网页不会处理。收藏夹会自动创建，如果已存在会直接使用，不会导致覆盖。此功能主要基于：如果一个网页需要频繁访问且未被拉入黑名单及证明其重要性，可配合Alfred等软件使用。

### 安装方法

项目当前暂无提交Chrome Store的计划，请使用以下方式安装。

下载地址：https://github.com/ZDL-Git/browse-manager/releases/latest

方法一：按gif步骤选择最新版本安装

<img src="https://github.com/ZDL-Git/resources-store/blob/master/gifs/installation-guide-compressed.gif" width="100%" />

重要说明：下载后先将压缩包解压，然后将文件夹名称中的版本号删除掉，打开chrome开发者模式，将文件夹拖入即安装成功。

升级时用新版本文件夹修改名称后覆盖掉原有的文件夹即可。【必须保证同位置同名称覆盖，且不要删除原版本的插件，否则会导致历史数据丢失】

方法二：clone仓库，平时可git pull更新获取最新的版本

#### 联系方式

如遇到安装或者使用问题，可选以下联系方式联系我，欢迎

QQ: 1226323187

Email: zdl_daily@163.com

提交bug: [Github issue](https://github.com/ZDL-Git/browse-manager/issues)

### 注意事项

* 由于是在后台js中listen事件，黑名单功能当前模式：在新tab打开黑名单网页时，会自动将这个tab关闭掉；在当前tab打开黑名单网页时，会自动后退到上一个非黑名单网页。如果环境对tab的管理要求严格，请谨慎使用。

* 打开“在页面显示访问次数”功能后，程序会在访问的页面临时嵌入一个fixed定位的div，使用完后会接着自动remove掉。

* 将网页加入黑名单时，如果其在收藏夹中，则会自动删除收藏。

## 大家如果用了请点个星星，让我知道如果不兼容升级会被多少个人揍，好吧！如果觉得不好用可以回来再把星星撤走😄
