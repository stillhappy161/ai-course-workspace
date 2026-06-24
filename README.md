# AI 课程开发智能体工作包

## 这是什么

一个为「企业AI落地商业课程」开发而构建的智能体协作工作包。三个人、异步协作、AI辅助。

## 快速开始（5分钟）

### 前置条件
1. 安装 [VS Code](https://code.visualstudio.com/)
2. 安装 Claude Code 扩展（在 VS Code 扩展商店搜索 "Claude Code"）
3. 确保 Claude Code 可以正常使用（打开 VS Code，在对话框里打字即可）

### 克隆仓库
```bash
git clone [仓库地址] ai-course-workspace
cd ai-course-workspace
code .
```

### 第一次对话
在 VS Code 对话框中输入：**"帮我做学习诊断"**

智能体会读取你的学习路线图，和你对话了解你当前的AI认知水平，给出诊断报告和下一步建议。

---

## 日常操作

### 看今日简报
```
今日简报
```
智能体扫描知识库 + 联网搜索 → 输出今日学习推荐和课程素材

### 存素材
```
存一下：[粘贴文章内容、链接、播客摘要、你的想法]
```
智能体自动结构化归档、标注来源、追问补充

### 提问学习
```
给我讲讲[某个概念]，用老板能听懂的话
```
智能体回答 + 追问 → 苏格拉底式引导

### 生成课程
```
生成模块X的内容
```
智能体扫描知识库 → 按模板生成PPT内容 → 等你审核

### 本周汇总
```
本周汇总
```
智能体汇总三人贡献、去重、标矛盾、标缺口

---

## 目录结构

```
ai-course-workspace/
├── README.md                    ← 你在这里
├── CLAUDE.md                    ← 智能体人设和行为规则（核心文件）
├── .claude/settings.json        ← 定时推送等配置
│
├── members/                     ← 三人个人空间
│   ├── 你/                      ← 学习路线 + 提问日志 + 周目标
│   ├── 合伙人A/
│   └── 研究生B/
│
├── knowledge-base/              ← 13个知识库分类文件（三人共用）
│   ├── cases-retail.md          # 零售案例
│   ├── cases-manufacturing.md   # 制造案例
│   ├── cases-other.md           # 其他行业案例
│   ├── frameworks.md            # AI框架与模型
│   ├── stats-data.md            # ROI数据与统计
│   ├── stories-quotes.md        # 金句与故事
│   ├── exec-pain-points.md      # 高管痛点
│   ├── exercises-discussions.md # 互动与讨论
│   ├── competitor-courses.md    # 竞品课程
│   ├── analogies.md             # 跨领域类比
│   ├── learning-materials.md    # 学习材料
│   ├── concept-cards.md         # 概念卡片
│   └── CONTRIBUTORS.md          # 贡献者信息
│
├── course-output/               ← 课程产出
│   ├── course-structure.md      # 课程大纲
│   └── module-templates/        # 模块模板
│
├── tasks/                       ← 任务卡片
│   └── week-1-sprint.md         # 第一周冲刺任务
│
├── scripts/                     ← 快捷指令说明
│   ├── daily-briefing.md
│   ├── feed-material.md
│   ├── generate-module.md
│   └── merge-weekly.md
│
└── weekly-digest/               ← 每周汇总（智能体自动生成）
```

---

## 协作规范

1. **每天提交一次**到 GitHub（晚上提交即可）
2. **每条素材标注贡献者**：`[贡献者: xxx] [日期: yyyy-mm-dd]`
3. **修改他人素材**：保留原作者，追加 `[修改: xxx] [日期]`
4. **遇到矛盾不要删**：标注 `⚡ 观点冲突`
5. **状态标签**：`#可入课` / `#待验证` / `#仅参考` / `#备选`

---

## 当前状态

- **阶段**：Week 1 冲刺模式（2026-06-23 ~ 2026-06-29）
- **目标**：完成知识库初始化 + 课程大纲V1 + PPT初稿
- **课程**：《从0到1搭建企业AI能力》
- **受众**：企业高管、老板
