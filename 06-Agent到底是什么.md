# 第6课：Agent 到底是什么？

## 先说结论

一句话：

> Agent = 能够主动完成任务的 AI 助手。

---

# 为什么 Agent 会出现？

先看传统 ChatGPT。

例如：

你问：

```text
苹果公司怎么样？
```

ChatGPT 回答。

---

然后结束。

---

本质上：

```text
你问
↓
它答
↓
结束
```

---

这叫：

```text
Chat
```

聊天模式。

---

# Agent 不一样

Agent 更像：

```text
实习生
```

而不是：

```text
百科全书
```

---

例如你说：

> 帮我分析苹果公司。

---

Agent 会想：

```text
需要查股价
需要查新闻
需要查财报
需要整理结果
```

---

于是：

```text
查资料
↓
整理
↓
分析
↓
输出报告
```

---

整个过程可能持续：

```text
30秒
5分钟
30分钟
```

---

这就是 Agent。

---

# Agent 和 ChatGPT 的区别

## ChatGPT

```text
问
↓
答
```

---

## Agent

```text
目标
↓
规划
↓
执行
↓
检查
↓
完成
```

---

Agent 多了：

```text
规划
执行
```

两个步骤。

---

# Agent 的组成部分

其实 Agent 并不神秘。

我们已经学过它的大部分零件。

---

## 大脑

```text
LLM
```

例如：

```text
ChatGPT
Claude
Gemini
```

---

负责：

```text
思考
推理
规划
```

---

## 工具

来自：

```text
API
```

---

例如：

```text
天气
邮件
搜索
数据库
```

---

负责：

```text
获取信息
执行动作
```

---

## 记忆

来自：

```text
数据库
```

---

负责：

```text
保存历史
保存结果
```

---

## 工作环境

来自：

```text
Workspace
```

---

负责：

```text
读取文件
修改文件
```

---

## 安全边界

来自：

```text
Docker
```

---

负责：

```text
隔离风险
限制权限
```

---

# 放到地图里

```text
Agent
├── LLM
├── API
├── Database
├── Workspace
└── Docker
```

---

所以：

> Agent 不是一个单独的新东西。

而是之前学过的东西组合在一起。

---

# 一个真实例子

假设未来你做：

```text
投资分析Agent
```

---

你说：

> 分析苹果公司。

---

Agent：

```text
调用股票API
↓
调用新闻API
↓
整理数据
↓
写分析报告
↓
存入数据库
```

---

以后再次分析：

```text
读取历史记录
↓
进行比较
```

---

这已经不是聊天。

而是在工作。

---

# 当前地图

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
```

---

# 今天最重要的三个概念

### Agent

```text
能够主动完成任务的 AI
```

---

### ChatGPT

```text
偏聊天
```

---

### Agent

```text
偏执行
```

---

所以：

```text
ChatGPT
=
回答问题

Agent
=
完成任务
```
