# 第11课：权限（Permission）到底是什么？

## 先说结论

一句话：

> 权限 = 某个人或某个程序被允许做什么事情。

---

# 三种最重要权限

## Read（读）

允许：

- 查看
- 读取
- 搜索

---

## Write（写）

允许：

- 创建
- 修改
- 删除

---

## Execute（执行）

允许：

- 运行程序
- 执行命令

---

# Agent 为什么需要权限

Agent 会：

- 读文件
- 改文件
- 执行命令

所以：

Agent能力越强

权限越重要。

---

# 最小权限原则

Principle of Least Privilege

意思：

> 只给完成任务所需的最小权限。

---

# Permission 和 Docker

Docker：

限制环境

Permission：

限制行为

---

所以：

Docker = 房间

Permission = 钥匙

---

# 当前地图

Git
↓
Workspace
↓
Docker
↓
Database
↓
API
↓
Agent
↓
MCP
↓
Codex
↓
Claude Code
↓
Cursor
↓
Permission

---

# 今天最重要的三个概念

### Read

读取权限

### Write

修改权限

### Execute

执行权限

---

所以：

Agent 的能力决定它能做什么。

Permission 决定它被允许做什么。
