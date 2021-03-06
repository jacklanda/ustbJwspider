﻿### ~~项目~~起源 （辣鸡代码，谈不上「项目」）

___

假期宅家闲散，整日足不出户，

适逢学校要求选课，选课所使用的「USTB本科教学网（vpn途径访问）」渲染太多，加载较慢。

这一点对家里网络环境较差的选课学生（我）不够友好，

加上自己宅家实在无聊，于是，便萌生出了写一个能够替代浏览器的自动选课脚本的想法。

### ~~项目~~现状

---

脚本的最初目的很简单：

即「帮助本校同学迅速地获知实时的可选公选课的相关信息，并针对自己喜欢的课程去重复地进行选课尝试」，

重复的选课尝试功能是由脚本自动实现的，这一点无须使用者上心。

使用者在启动脚本后仅需根据提示来键入相关的登陆&选课信息，等待选课结果即可。

此外，脚本目前已基本实现了：自动选课&退课，自动获取课程表、创新学分、以及课程成绩等一切原网站所能够获取的个人数据并清洗入库。

另：脚本中涉及的个人账号&密码将不以任何形式存储在任何实体中；

​		脚本概不提供各请求所涉及到的任何 api，烹饪菜谱已备齐，请食用者自行获取原食材

### 使用指南

---

#### 安装依赖

如果你想体验脚本的功能，请按如下步骤进行：

（默认使用者已安装CPython37以上的相关 [Python](https://www.python.org/) 发行版）

* 进入ustbJwspider根目录下，启动cmd命令行/Terminal/shell，键入：

```python
pip3 install -r requirements.txt                    #使用pip安装
```

* 自行到 MongoDB 官网上下载适配自己系统版本的 [MongoDB](https://www.mongodb.com/download-center/community) 安装包，解压安装

  到 RoboStudio 官网下载 [Robo3T](https://robomongo.org/download)（GUI），安装后打开GUI，建立位于本地的MongoClient

#### 使用脚本

进入ustbJwspider根目录下，运行app.py文件，根据操作提示键入相关信息即可。

### 运行截图

---

- [x]  ***脚本登陆***

![](https://i.imgur.com/wM2k6Pb.png)

- [x]  ***功能选择***

![](https://i.imgur.com/zbSZ7rI.png)

- [x]  ***尝试选课***

![](https://i.imgur.com/cwKnzRm.png)

- [x]  ***尝试退课***

![](https://i.imgur.com/2FhoSBJ.png)

### 已知问题

---

* 代码繁冗，有待重构&封装
* 脚本在「与用户交互」方面优化不足

### To-do List

---

* GUI
* 针对个人成绩进行数据可视化分析
* 部署至VPS，将各功能封装为可替代原网址内容的接口
* ~~spider有夸大的嫌疑，应将项目更名为：ustbJwcrawler~~

### 交流沟通

---

由于作者水平有限，在脚本执行的过程中，难免会出现这样或那样的问题，

除了目前已发现的问题外，若脚本由于别的原因而屡次报错，欢迎来提Issue 和 PR (〃'▽'〃)。

### 版本历史

---


* 0.1.2
    * 实现选课和退课功能
* 0.1.1
    * 实现公选课数据的清洗&入库
    * 实现登陆&选课的交互逻辑
* 0.1.0
    * main()编写完成


### LICENSE

---

[MIT License](https://github.com/jacklanda/ustbJwspider/blob/master/LICENSE)