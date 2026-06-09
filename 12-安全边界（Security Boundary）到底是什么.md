# 第12课：安全边界（Security Boundary）到底是什么？

## 先说结论

一句话：

> 安全边界 = AI 能够影响范围的边界。

---

# Workspace

Workspace = 物理边界

决定：

AI能接触什么

---

# Permission

Permission = 行为边界

决定：

AI能做什么

---

# Docker

Docker = 环境边界

决定：

AI在哪里做事

---

# MCP

MCP = 工具边界

决定：

AI能连接什么系统

---

# 安全边界地图

Workspace
↓
决定能看到什么

Permission
↓
决定能做什么

Docker
↓
决定在哪里做

MCP
↓
决定连接什么

---

# Agent 与边界

强Agent
+
弱边界
=
高风险

---

强Agent
+
强边界
=
可控

---

# 今天最重要的三个概念

### Workspace

看到什么

### Permission

能做什么

### Security Boundary

把风险控制在范围内

---

所以：

AI 安全的核心不是相信 AI 不会犯错。

而是设计好边界，让它即使犯错，影响也有限。
