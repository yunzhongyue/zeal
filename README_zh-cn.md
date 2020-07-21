# Zeal

[![Changelog](https://img.shields.io/github/release/zealdocs/zeal.svg?style=flat-square)](https://github.com/zealdocs/zeal/releases)
[![Gitter](https://img.shields.io/gitter/room/zealdocs/zeal.svg?style=flat-square)](https://gitter.im/zealdocs/zeal)
[![IRC](https://img.shields.io/badge/chat-on%20irc-blue.svg?style=flat-square)](https://kiwiirc.com/client/irc.freenode.net/#zealdocs)
[![Telegram Channel](https://img.shields.io/badge/follow-on%20telegram-179cde.svg?style=flat-square)](https://telegram.me/zealdocs)
[![Twitter](https://img.shields.io/badge/follow-on%20twitter-1da1f2.svg?style=flat-square)](https://twitter.com/zealdocs)

[![AppVeyor](https://img.shields.io/appveyor/ci/zealdocs/zeal/master.svg?style=flat-square)](https://ci.appveyor.com/project/zealdocs/zeal)
[![Coverity Scan](https://img.shields.io/coverity/scan/4271.svg?style=flat-square)](https://scan.coverity.com/projects/4271)

Zeal 是一个简单的离线文档浏览器，灵感来自于 [Dash](https://kapeli.com/dash).

![Screenshot](https://images.gitee.com/uploads/images/2020/0721/221342_d174eccd_23532.png "2020-07-21_22-13.png")

## 下载

从  [下载页](https://zealdocs.org/download.html) 获取适用于window和linux的二进制发行包.

## 如何使用

安装后点击 `工具->文档集`, 选择一个你想要的, 然后点击 `下载` 按钮.

## 如何构建

### 构建依赖

* [CMake](https://cmake.org/).
* [Qt](https://www.qt.io/)  5.9.5 版本 或 以上. 需要模块: Qt WebEngine Widgets.
* [libarchive](https://libarchive.org/).
* [SQLite](https://sqlite.org/).
* 仅 X11平台: Qt X11 Extras 和 `xcb-util-keysyms`.

### 构建说明

```sh
cmake -B build
cmake --build build
```

可以从 [wiki](https://github.com/zealdocs/zeal/wiki) 获取更多的说明信息.

## 查询 & 过滤文档集

您可以通过使用":"指示所需的文档集来限制搜索范围:

`java:BaseDAO`

你可以使用逗号分割多个文档集:

`python,django:string`

## 命令行

如果愿意，可以从命令行通过查询启动Zeal：

`zeal python:pprint`

## 创建你自己的文档集

按照 [Dash docset generation guide](https://kapeli.com/docsets) 中的说明进行操作.

## 联系和支持

我们需要你的反馈！下面列出了联系开发人员和请求帮助的不同方法：
* 到 [GitHub issues](https://github.com/zealdocs/zeal/issues) 提交BUG或特性需求.
* 和开发者或其他热心网友在 [Gitter](https://gitter.im/zealdocs/zeal) 或者 [Freenode](https://freenode.net/) 下的 IRC 频道 #zealdocs 进行交流.
* 在 [Google Group](https://groups.google.com/d/forum/zealdocs) 提问题. 你可以发送邮件到 zealdocs@googlegroups.com.
* 别忘了在Twitter关注 [@zealdocs](https://twitter.com/zealdocs) !
* 最后，如需私人通信，请发送电子邮件至 zeal@zealdocs.org.

## 许可证

本软件根据GNU通用公共许可证版本3（GPLv3）的条款进行授权。 许可证全文可以在 [COPYING](https://github.com/zealdocs/zeal/blob/master/COPYING) 文件或 [在线](https://www.gnu.org/licenses/gpl-3.0.html) 查阅.
