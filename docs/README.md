# 项目文档总览

## 1. 目标

这个目录的作用，是把项目文档按“策略、生产、互动、自动化、设计”分层。

原则：

- 稳定的方向和判断，放在策略层
- 可重复执行的流程，放在生产层
- 可直接复用的回复知识，放在互动层
- 供 AI 或脚本调用的说明，放在自动化层
- 单篇配图说明，放在设计层

---

## 2. 当前结构

```text
docs/
├── README.md
├── automation/
│   └── knowledge-map.md
├── design/
│   └── canva-design-guide.md
├── interaction/
│   └── comment-library.md
└── production/
    └── content-production-guide.md
```

---

## 3. 每层放什么

### 3.1 策略层

主文件：

- 根目录 `README.md`

放这里的内容：

- 账号定位
- 用户画像
- 主题记忆库
- 数据复盘
- 内容规划
- 商业化方向

特点：

- 变化相对慢
- 决定“做什么”和“为什么做”

### 3.2 生产层

主文件：

- `docs/production/content-production-guide.md`

放这里的内容：

- 选题流程
- 判重规则
- 写作标准
- 配图拆页规范
- 发布前检查
- 发布后复盘动作

特点：

- 变化频率中等
- 决定“怎么做”

### 3.3 互动层

主文件：

- `docs/interaction/comment-library.md`

放这里的内容：

- 评论分类
- 回复原则
- 回复模板
- 风险分级
- 自动化字段

特点：

- 为评论回复和粉丝互动服务
- 要尽量标准化、便于 AI 调用

### 3.4 自动化层

主文件：

- `docs/automation/knowledge-map.md`

放这里的内容：

- 不同自动化任务需要读取哪些文档
- 输入输出建议
- 字段约定
- 任务边界和人工确认点

特点：

- 为后续 AI 工作流和脚本提供路由

### 3.5 设计层

主文件：

- `docs/design/canva-design-guide.md`

放这里的内容：

- 通用 Canva 配图规范
- 仓库素材使用规则
- 页数与拆页节奏
- 设计复用建议

特点：

- 面向所有内容的通用执行
- 不承担账号策略判断

---

## 4. 推荐使用顺序

如果是写新内容：

1. 先看根目录 `README.md`
2. 再看 `docs/production/content-production-guide.md`
3. 再写 `content/DayN.md`
4. 需要做图时看 `docs/design/`

如果是做评论回复：

1. 先看 `docs/interaction/comment-library.md`
2. 再看根目录 `README.md` 中的人设和互动原则
3. 输出回复建议

如果是做自动化：

1. 先看 `docs/automation/knowledge-map.md`
2. 再按任务类型读取对应文档

---

## 5. 后续建议补充

后续如果开始做更系统的数据和自动化，可以继续新增下面两类文件：

- `data/`：存放结构化数据，例如发布数据、评论样本、选题池
- `docs/design/templates/`：沉淀通用 Canva 模板说明

目前阶段先不急着加太多空目录，保持够用、清楚、好维护。
