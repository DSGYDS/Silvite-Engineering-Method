# Silvite Engineering Method

一套面向真实软件工程任务的 Agent Skill，用来约束 Agent 如何规划、执行、验证和迭代工作。

它从长期、高强度的 Agent-native 软件工程实践材料中提炼，并通过压力场景持续校正。当前版本关注工程决策，而不是某个项目、语言、框架或平台。

## 适用场景

- 多模块、跨端或跨平台修改
- 生产故障、高风险迁移和失败恢复
- 架构调整、插件边界与复杂度控制
- 自动化、智能控制和权限逐级扩大
- 陌生技术栈、系统建模和项目驱动学习
- 测试不完整、完成状态不确定或需要明确证据

它可以用于 Web、Desktop、Mobile、Backend、Embedded、CLI、Libraries、Networking，以及普通单端或大型系统工程。

## 它不是什么

- 不是某个项目的内部文档或商业计划
- 不是个人经历、成长指南或 AI 哲学文章
- 不是单一技术栈教程
- 不是对所有项目都适用的“终极方法论”
- 不替代领域安全规范、组织审批或专业判断

## 安装与使用

将整个目录复制到 Agent 宿主支持的 Skills 目录。例如 Codex 可放入：

```text
$CODEX_HOME/skills/silvite-engineering-method/
```

如果未设置 `CODEX_HOME`，可使用宿主文档指定的默认 Skills 目录。安装后显式调用 `$silvite-engineering-method`，或让支持自动发现的宿主在符合触发条件时加载它。

示例请求：

```text
使用 $silvite-engineering-method 规划这次跨模块修改，先定义边界、失败模式、回滚和完成证据。
```

## 仓库结构

- `SKILL.md`：精炼的触发条件与核心决策流程
- `references/`：边界、验证、复杂度、系统思维和恢复细节
- `evals/`：压力场景、行为评分方法与脱敏结果
- `UPDATE_GUIDE.md`：如何从新案例更新规则
- `PUBLICATION_CHECKLIST.md`：公开安全门

## 更新与反馈

更新前先阅读 [UPDATE_GUIDE.md](UPDATE_GUIDE.md)。反馈最好包含：真实问题、Agent 的原始选择、可观察后果、缺失规则或反例，以及可公开的验证证据。不要提交密钥、用户数据、内部拓扑、私有代码或未公开商业/技术事实。

## 当前成熟度

当前为 **v0.1.0**：体系仍在快速变化，已完成的初始压力测试见 [evals/results-v0.1.md](evals/results-v0.1.md)，但尚未经历足够多独立项目与长期运行验证。达到 v1.0 前，任何规则都应允许被反例和新证据修正。

本仓库采用 [MIT License](LICENSE)。
