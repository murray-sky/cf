<p align="center">
<img width="500" src="https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202207022209168.png"><br><br>
<a href="https://github.com/teamssix/cf/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/teamssix/cf"/></a>
<a href="https://github.com/teamssix/cf/releases"><img alt="GitHub issues" src="https://img.shields.io/github/release/teamssix/cf"/></a>
<a href="https://github.com/teamssix/cf/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/></a>
<a href="https://github.com/teamssix/cf/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/teamssix/cf/total?color=brightgreen"/></a>
<a href="https://goreportcard.com/report/github.com/teamssix/cf"><img alt="Go Report Card" src="https://goreportcard.com/badge/github.com/teamssix/cf"/></a>
<a href="https://twitter.com/intent/tweet/?text=CF%2C%20an%20amazing%20cloud%20exploitation%20framework%0Ahttps%3A%2F%2Fgithub.com%2Fteamssix%2Fcf%0A%23cloud%20%23security%20%23cloudsecurity%20%23cybersecurtiy"><img alt="tweet" src="https://img.shields.io/twitter/url?url=https://github.com/teamssix/cf" /></a>
<a href="https://twitter.com/teamssix"><img alt="Twitter" src="https://img.shields.io/twitter/follow/teamssix?label=Followers&style=social" /></a>
<a href="https://github.com/teamssix"><img alt="Github" src="https://img.shields.io/github/followers/TeamsSix?style=social" /></a><br></br>
中文 | <a href="README_EN.md">English</a>
</p>



---

CF 是一个云环境利用框架，适用于在红队场景中对云上内网进行横向、SRC 场景中对 Access Key 即访问凭证的影响程度进行判定、企业场景中对自己的云上资产进行自检等等。

CF 下载地址：[github.com/teamssix/cf/releases](https://github.com/teamssix/cf/releases)

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737418.png)

当前已支持的云：

- [x] 阿里云
- [x] 腾讯云
- [ ] AWS（预计在 2022 年 10 月 14 日前支持）
- [ ] 华为云（预计在 2022 年 12 月 14 日前支持）

功能排期可参考：[github.com/teamssix/cf/discussions/130](https://github.com/teamssix/cf/discussions/130)

## 使用手册

使用手册请参见：[wiki.teamssix.com/cf](https://wiki.teamssix.com/cf)

[![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209081100625.png)](https://wiki.teamssix.com/cf)

## 使用案例

|                标题                | 使用 CF 的版本 |             文章地址              | 发布时间  |
| :--------------------------------: | :------------: | :-------------------------------: | :-------: |
| 《记录一次平平无奇的云上攻防过程》 |     v0.4.0     |  https://zone.huoxian.cn/d/2557   | 2022.9.14 |
|   《我用 CF 打穿了他的云上内网》   |     v0.2.4     | https://zone.huoxian.cn/d/1341-cf | 2022.7.13 |

## 简单上手

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737405.png)

> 这里以阿里云为例，其他更多操作可以查看上面的使用手册。

配置访问配置

```bash
cf config
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737407.png)

一键列出当前访问凭证的权限

```bash
cf alibaba perm
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737408.png)

一键接管控制台

```bash
cf alibaba console
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737409.png)

一键列出当前访问凭证的云服务资源

```bash
cf alibaba ls
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737410.png)

查看 CF 为实例执行命令的操作的帮助信息

```bash
cf alibaba ecs exec -h
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737411.png)

一键为所有实例执行三要素，方便 HVV

```bash
cf alibaba ecs exec -b
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737412.png)

一键获取实例中的临时访问凭证数据

```bash
cf alibaba ecs exec -m
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737413.png)

一键下载 OSS 对象存储数据

```bash
cf alibaba oss obj get
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737414.png)

一键升级 CF 版本

```bash
cf upgrade
```

![](https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202209071737416.png)

如果感觉还不错的话，师傅记得给个 Star 呀 ~，另外 CF 的更多使用方法可以参见使用文档：[wiki.teamssix.com/cf](https://wiki.teamssix.com/cf)

## 贡献者

十分感谢各位师傅对 CF 的贡献~，如果你也想对 CF 贡献代码，请参见贡献说明：[CONTRIBUTING](https://github.com/teamssix/cf/blob/main/CONTRIBUTING.md)

<div align=center>
<table>
    <tr>
        <td align="center"><a href="https://github.com/teamssix"><img alt="TeamsSix"
                                src="https://avatars.githubusercontent.com/u/49087564?v=4" style="width: 100px;"/><br/>TeamsSix</a></td>
        <td align="center"><a href="https://github.com/Amzza0x00"><img alt="Amzza0x00"
                                src="https://avatars.githubusercontent.com/u/32904523?v=4"  style="width: 100px;"/><br/>Amzza0x00</a></td>
        <td align="center"><a href="https://github.com/Esonhugh"><img alt="Esonhugh"
                                src="https://avatars.githubusercontent.com/u/32677240?v=4"  style="width: 100px;"/><br/>Esonhugh</a></td>
        <td align="center"><a href="https://github.com/Dawnnnnnn"><img alt="Dawnnnnnn"
                                src="https://avatars.githubusercontent.com/u/24506421?v=4"  style="width: 100px;"/><br/>Dawnnnnnn</a></td>
        <td align="center"><a href="https://github.com/Belos-pretender"><img alt="Belos-pretender"
                                src="https://avatars.githubusercontent.com/u/52148409?v=4"  style="width: 100px;"/><br/>Belos-pretender</a></td>
</table>
</div>

<div align=center><a href="https://github.com/teamssix"><img src="https://repobeats.axiom.co/api/embed/30b8de6c059cbe83fe0ba44fff91136270a39ab9.svg"></a></div>



## 404星链计划

<img src="https://github.com/knownsec/404StarLink/raw/master/Images/logo.png" width="40%">

CF 现已加入 [404星链计划](https://github.com/knownsec/404StarLink)


## 更多

如果你对云安全比较感兴趣，可以看我的另外一个项目 [Awesome Cloud Security](https://github.com/teamssix/awesome-cloud-security)，这里收录了很多国内外的云安全资源。

另外在我的[云安全文库](https://wiki.teamssix.com/)里有大量的云安全方向的笔记和文章，最后，下面这个是我的个人微信公众号，欢迎关注 ~

<div align=center><a href="https://github.com/teamssix"><img width="700" src="https://cdn.jsdelivr.net/gh/teamssix/BlogImages/imgs/202204152148071.png"></a></div>

**有想法一起研究的师傅可以投递简历至 admin@wgpsec.org 加入狼组安全团队。**

<div align=center><a href="https://github.com/teamssix"><img src="https://api.star-history.com/svg?repos=teamssix/cf&type=Timeline"></a></div>

## 注意事项

* 本工具仅用于合法合规用途，严禁用于违法违规用途。
* 本工具中所涉及的风险点均属于租户责任，与云厂商无关。
