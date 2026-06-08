# 第3课：Docker（容器）到底是什么？

这一课非常重要。

因为你以后会经常看到：

```text
Docker
Container
Sandbox
隔离环境
```

如果不理解 Docker，会感觉这些词都很抽象。

实际上它们都在解决同一个问题：

> 如何让 AI 安全地工作。

---

# 先说结论

一句话：

> Docker = 给程序准备的独立工作房间。

---

## 从 Workspace 继续讲

上一课我们学过：

```text
Repo
=
档案室

Workspace
=
办公桌
```

---

现在出现一个问题。

假设你请了一位实习生。

让他在办公桌工作。

---

正常情况：

```text
办公桌
↓
修改项目
```

没问题。

---

但如果实习生很粗心：

```text
删除文件
修改系统设置
乱装软件
```

怎么办？

---

于是你给他安排一个单独的小房间。

房间里：

```text
桌子
电脑
项目资料
```

都有。

但是：

```text
出不了房间
```

---

这就是 Docker。

---

# Docker 的本质

很多教程会说：

```text
Docker 是容器技术
```

对于初学者帮助不大。

---

你可以先理解成：

```text
Docker
=
独立工作房间
```

---

程序进入房间以后：

可以：

```text
读文件
写文件
运行程序
```

---

但是默认只能碰：

```text
房间里的东西
```

---

碰不到：

```text
你的电脑
你的照片
你的银行资料
```

---

# 为什么 Docker 会出现？

因为直接在电脑上运行程序风险太大。

---

例如：

你从网上下载一个程序。

运行它。

---

它理论上可以访问：

```text
桌面
下载目录
文档目录
```

甚至更多。

---

所以成熟实践会说：

```text
不要直接运行
```

而是：

```text
放进 Docker
```

---

这样程序即使出问题。

影响范围也被限制住了。

---

# Docker 和 Workspace 的关系

很多人会混淆。

实际上：

```text
Workspace
=
工作桌

Docker
=
工作房间
```

---

关系是：

```text
Docker
└── Workspace
```

---

例如：

```text
Docker容器
└── AI项目
```

---

AI 实际工作：

```text
Workspace
```

---

Workspace 所在的位置：

```text
Docker
```

---

# 为什么 AI Coding 工具喜欢 Docker？

因为 AI 会：

```text
读文件
改文件
运行命令
安装依赖
```

---

这些动作都有风险。

---

例如你说：

> 帮我启动项目。

AI 可能执行：

```text
npm install
```

或者：

```text
pip install
```

---

如果直接在电脑运行。

有可能：

```text
污染环境
安装错误版本
修改配置
```

---

而 Docker 里：

```text
坏了
↓
删掉容器
↓
重新创建
```

结束。

---

# 一个非常重要的概念

## 可隔离

什么意思？

假设 AI 搞坏了环境。

---

没有 Docker：

```text
你的电脑坏了
```

---

有 Docker：

```text
容器坏了
```

---

删除容器：

```text
重新创建
```

即可。

---

所以：

> Docker 提供隔离。

---

# 为什么很多 AI 产品都强调 Sandbox？

你以后会经常看到：

```text
Sandbox
```

中文：

```text
沙盒
```

---

其实可以理解成：

```text
受限制的小环境
```

---

Docker 经常被拿来实现沙盒。

---

所以：

```text
Sandbox
```

不是 Docker。

但：

```text
很多 Sandbox
↓
使用 Docker 实现
```

---

# 回到 Codex

你最开始问过：

> 为什么推荐独立 Workspace？

现在答案升级了。

---

第一层：

```text
Workspace
=
限制AI看到什么
```

---

第二层：

```text
Docker
=
限制AI能碰什么
```

---

这两个概念配合：

```text
Docker
└── Workspace
```

就形成了比较安全的环境。

---

# 真实项目里是什么样？

很多成熟团队：

```text
GitHub Repo
↓
Docker
↓
Workspace
↓
AI Agent
```

---

AI 实际看到的是：

```text
项目代码
```

---

看不到的是：

```text
个人照片
银行资料
其它项目
```

---

这就是：

```text
最小权限原则
```

的体现。

---

# 今天最重要的三个概念

### Docker

```text
独立工作房间
```

---

### Container（容器）

```text
Docker创建出来的房间
```

---

### Sandbox（沙盒）

```text
受限制的安全环境
```

很多时候用 Docker 实现。

---

# 小测验

假设你让 AI 帮你修改网站。

下面哪个更安全？

### A

```text
AI
↓
直接访问整个电脑
```

---

### B

```text
AI
↓
Docker容器
↓
Workspace
↓
网站项目
```

如果理解了今天的内容，你应该会发现：

> Workspace 解决“看什么”的问题。
>
> Docker 解决“能碰什么”的问题。

这就是为什么很多 AI Coding 工具都会强调：

```text
Container
Sandbox
Isolated Environment
```
