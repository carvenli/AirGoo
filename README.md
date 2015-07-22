# AirGoo

一个提供访问Google搜索的反向代理程序。

## FAQ

- 这玩意能干啥？

> 为了能任性的能基本愉快的使用Google搜索、图片、地图。

- 原理和工作模式？

> ![AirGoo](https://i.imgur.com/nU5lCui.png)

- 那XXX也能反代，为什么要写app？

> 要能“基本可用”“基本愉快”的Googling，需要处理因反代而带来的域及资源等很多麻烦问题，为了实现这个反代谷歌的最低水准，写app是实现复杂处理的较容易方法，也才能完整妥善的处理好资源问题。

- 似乎挺费内存？

> 目前只有Node.js实现版本，可能需要几十到一百兆内存，未来可能会增加其它语言的实现，或许可以更快的释放内存占用。内存不被利用就是浪费资源，总比大量的使用I/O要好的多。虽然内存不是白菜价但还是消费品水平，升级配置才是根本。

- 能不能去广告换标识？

> 除了去除链接的二次跳转，原样还原，原样传输，不更改具体业务数据。

- 为什么Google其它产品就不能愉快使用？

> Google产品线很庞大很复杂，只能覆盖到搜索图片地图这些基本服务。

- 可以不用nginx等吗？

> 当然可以，只是无法利用到nginx提供的cache、https/spdy等特性了。

## Usage

阅读项目Wiki了解用法及配置。

## ChangeLog

V1.1.5 - 15/7/22

- 修复了部分资源处理不干净的问题
- 调整了在abusing时的处理
- 更新了readme

**注**: 本次更新需要清理中间缓存、浏览器缓存。
