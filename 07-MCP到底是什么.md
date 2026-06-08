# 第7课：MCP（Model Context Protocol）到底是什么？

## 先说结论

一句话：

> MCP = Agent 连接外部工具的统一标准。

---

# MCP 出现之前

假设你做一个 Agent。

希望它能够访问：

```text
GitHub
数据库
Notion
邮箱
日历
Slack
```

---

以前怎么办？

每接一个系统：

```text
Agent
↓
单独开发接口
```

---

例如：

```text
Agent
↓
GitHub API
```

---

再来一个：

```text
Agent
↓
Notion API
```

---

再来一个：

```text
Agent
↓
Google Calendar API
```

---

于是最后：

```text
Agent
├── GitHub API
├── Notion API
├── Calendar API
├── Gmail API
└── ...
```

---

问题来了。

每个系统：

```text
认证方式不同
参数不同
返回格式不同
```

---

开发成本越来越高。

---

# 用现实世界理解

假设你去旅游。

---

美国：

```text
110V
```

---

中国：

```text
220V
```

---

英国：

```text
插头长得不一样
```

---

日本：

```text
标准又不一样
```

---

于是出现：

```text
万能转换器
```

---

不管去哪：

```text
设备
↓
转换器
↓
当地插座
```

---

这就是 MCP 的角色。

---

# MCP 的本质

你可以先理解成：

> AI 世界的 USB 接口标准。

---

为什么 USB 伟大？

因为：

```text
鼠标
键盘
摄像头
U盘
```

都能插。

---

不用每个设备单独设计接口。

---

MCP 也是一样。

---

# 没有 MCP

```text
Agent
↓
GitHub API

Agent
↓
Notion API

Agent
↓
Calendar API

Agent
↓
Gmail API
```

---

每个都单独接。

---

# 有 MCP

```text
Agent
↓
MCP
↓
各种工具
```

---

Agent 只学会：

```text
MCP
```

一种语言。

---

以后接什么工具：

```text
GitHub
Notion
数据库
邮件
日历
```

都统一。

---

# MCP 和 API 的关系

```text
API
=
电器

MCP
=
插座标准
```

---

API 仍然存在。

---

只是：

```text
MCP
统一管理API
```

---

# 一个真实例子

假设未来你做：

```text
AI投资助手
```

---

需要：

```text
读取GitHub
读取数据库
读取Notion
发送邮件
```

---

没有 MCP：

```text
写4套接口
```

---

有 MCP：

```text
接入4个MCP Server
```

即可。

---

# 什么是 MCP Server？

可以理解成：

> 某个工具提供的 MCP 入口。

---

例如：

```text
GitHub MCP Server
```

负责：

```text
读仓库
创建Issue
创建PR
```

---

例如：

```text
Notion MCP Server
```

负责：

```text
读页面
写页面
搜索内容
```

---

例如：

```text
数据库 MCP Server
```

负责：

```text
查询
写入
修改
```

---

# MCP 和 Agent 的关系

没有 MCP：

```text
Agent
=
会思考的人
```

---

有 MCP：

```text
Agent
=
会思考
+
会使用工具的人
```

---

所以：

> MCP 让 Agent 真正接触现实世界。

---

# 当前课程地图

```text
Git
↓
管理历史

Repo
↓
管理项目

Workspace
↓
工作区域

Docker
↓
隔离环境

Database
↓
保存数据

API
↓
连接系统

Agent
↓
完成任务

MCP
↓
统一连接工具
```

---

# 今天最重要的三个概念

### MCP

```text
Agent连接工具的统一标准
```

---

### API

```text
具体工具接口
```

---

### MCP

```text
统一管理API和工具
```

---

所以：

```text
Agent
↓
MCP
↓
API
↓
工具
```

形成现代 Agent 架构。
