---
title: 我的 Agent 学习之旅：从 invoke() 到智能体设计模式
published: 2026-08-11
description: 记录我从 LangChain 基础到《智能体设计模式》的学习路径，以及我对 Agent 开发的理解。
tags: [Agent, LangChain, 学习]
category: 技术
slug: agent-learning-journey
---

## 🧭 起点：一个很朴素的问题

几个月前，我对 AI 的印象还停留在"聊天机器人"。直到我第一次写出这样的代码：

```python
from langchain_openai import ChatOpenAI

model = ChatOpenAI(model="kimi-latest", api_key=key)
response = model.invoke("你好")
print(response.content)
```

那一刻我才意识到：原来我写的每一行代码，都可以变成"模型看得懂的指令"。也是从那一刻起，我踏上了 Agent 开发的学习之路。

## 📚 学习路径

### 第一阶段：LangChain 基础

- `chat_models` 初始化模型、`invoke()` / `stream()` 调用
- `BaseMessage` 四个子类（Human / AI / System / Tool）
- 用系统提示词实现结构化输出

这一阶段让我明白了：**模型本身不智能，是"提示 + 上下文"让它显得智能**。

### 第二阶段：《智能体设计模式》

学完基础后，我开始啃《智能体设计模式》这本书。印象最深的是几个核心模式：

| 模式 | 一句话理解 |
|---|---|
| 提示链 | 把大任务拆成小步骤，前一步的输出喂给后一步 |
| 路由 | 根据输入类型，动态选择处理路径 |
| 反思 | 让模型自己批判自己的输出，迭代改进 |
| 工具调用 | Agent 与外部世界交互的"手" |

**我的最大感悟**：Agent 开发的本质，不是写更复杂的代码，而是**设计更合理的"流程"**——把模型的强项（语言理解、推理）和工具的强项（执行、检索、计算）组合起来。

## 🎮 一点题外话

学习之余，我喜欢玩《明日方舟：终末地》和《崩坏：星穹铁道》。有时候觉得，学 Agent 开发和玩这类游戏有一种奇妙的共通点——都是在**理解一套系统的运作规则，然后想办法让它按你的意志运转**。

## 🏁 接下来

- 用 LangGraph 实现带记忆的完整 Agent
- 用 FastAPI 把自己的 Agent 包成 API 服务
- 把《智能体设计模式》里的模式一个个落地实践

路还很长，但星星就在那里。🚀
