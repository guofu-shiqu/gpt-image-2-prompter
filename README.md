# GPT-image-2 Prompter

为 GPT-image-2 和 ChatGPT 图像 2.0 设计、改写、诊断和迭代出图提示词的 Codex Skill。

## 用途

- 将粗略出图想法改写为结构化中文提示词。
- 为海报、样卡、产品图、课程图、角色设定、信息图和多图合成生成可执行提示词。
- 给出推荐参数、GPT-image-2 规则项、质感控制、检查点和单点迭代指令。
- 处理 PSD/分层拆分友好需求时，明确图像模型不会直接输出 PSD，并提供后期拆层建议。

## 目录

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── gpt-image-2-notes.md
    └── prompt-templates.md
```

## 安装

将本目录放到 Codex 技能目录中：

```bash
cp -R gpt-image-2-prompter ~/.codex/skills/
```

使用时可以直接点名：

```text
使用 $gpt-image-2-prompter，把我的出图想法改写成中文、可直接执行的 GPT-image-2 提示词。
```

## 维护原则

- 默认中文输出。
- 最终提示词必须包含 `GPT-image-2 rules:` 段落。
- 图片内文字优先保持短、准、可验证；长文案放回可编辑层。
- 不承诺直接生成 PSD 分层文件，只提供 PSD 拆层友好的视觉稿提示词和图层建议。
