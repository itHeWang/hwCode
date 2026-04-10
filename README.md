# Skill 仓库

这是一个用于存放和管理 OpenCode 自定义 Skills 的仓库。

## 什么是 Skill？

Skill 是 OpenCode 的扩展机制，允许用户自定义 AI 行为模式、技能和工作流。通过 Skill，你可以：

- 让 AI 具备特定领域的专业知识
- 自定义交互方式和回复风格
- 封装重复性的工作流程
- 优化特定任务的执行效率

## 包含的 Skills

### 1. my-chinese-assistant（中文开发助手）

专为中文开发者打造的助手技能。

**主要功能：**
- 代码中文注释生成
- 技术文档中英翻译
- 需求转代码（中文描述需求，直接生成代码）
- 错误信息中文解读

**适用场景：**
- 用户使用中文交流
- 需要中文代码注释或文档
- 技术问题解答和报错分析
- 代码实现需求

---

### 2. skill-creator（Skill 创建工具）

用于创建、测试和优化自定义 Skill 的完整工具链。

**主要功能：**
- 新建 Skill（从需求到实现）
- 改进现有 Skill
- 测试用例编写和运行
- 性能基准测试（Benchmark）
- Skill 描述优化（提升触发准确性）

**适用场景：**
- 从零创建新的 Skill
- 优化现有 Skill 的效果
- 评估 Skill 性能
- 批量测试和迭代改进

---

## 如何使用

### 安装 Skill

将 skill 目录复制到 OpenCode 的 skills 目录：
```
~/.agents/skills/<skill-name>/
```

### 触发 Skill

Skills 会根据描述自动触发。当任务匹配 skill 的描述时，AI 会自动使用对应的技能。

---

## 添加新 Skill

1. 在 `skills/` 目录下创建新文件夹
2. 添加 `SKILL.md` 文件，包含：
   - `name`: Skill 名称
   - `description`: 触发描述
   - 使用说明和功能文档
3. 提交到仓库

---

## 目录结构

```
skills/
├── my-chinese-assistant/
│   └── SKILL.md
└── skill-creator/
    └── SKILL.md
```