# OPC 诊室 · 多平台安装指南

[`prompt/diagnostician.md`](prompt/diagnostician.md) 里是一段**模型无关的提示词**,不是某个特定平台的专属功能。Claude / ChatGPT / DeepSeek / Gemini / Kimi / 通义千问等任何大模型都能跑——Skill 封装版只是为 Claude Code 用户提供的便利,装一次就能一键唤起,但**不是唯一方式**。

---

## 方式 A · 直接粘贴（任何大模型，最推荐）

适合:所有人。零配置,30 秒上手。

1. 复制 [`prompt/diagnostician.md`](prompt/diagnostician.md) 的全部内容
2. 打开任意大模型（Claude / ChatGPT / DeepSeek / Gemini / Kimi / 通义千问等）,新建对话
3. 粘贴进去,发送
4. 它就开始诊断了

> 就这么简单。诊断能力全在那段提示词里,不需要装任何东西。

---

## 方式 B · Claude Code Skill 封装（一键复用）

适合:Claude Code 用户。装一次,说一句"诊断我的项目"即自动唤起。

### 目录结构

```
skill/
├── SKILL.md                          # skill 定义(触发条件 + 如何使用)
├── diagnostician.md                  # 诊断官提示词全文
└── examples/                         # 4 个真实诊断案例(供 Claude 参考它该有的样子)
    ├── founder-self-diagnosis.md     # AI 创业工具:它如何诊断自己的作者
    ├── saas-founder-diagnosis.md     # SaaS:2000 免费用户只有 3 付费
    ├── ecommerce-diagnosis.md        # 电商:选品换三轮,每轮第一单后归零
    └── content-creator-diagnosis.md  # 内容创作者:粉丝卡 5000,广告被压价
```

### 安装

把整个 `skill/` 文件夹放进你的 skills 目录,Claude Code 会自动识别。之后在对话里说"诊断一下我的项目""我的产品卡在 XX,帮我看看"即可触发。

---

## 方式 C · Claude Project 自定义指令

适合:Claude.ai 网页端用户。

1. 新建一个 Claude Project
2. 把 `diagnostician.md` 的内容粘进 Project 的"自定义指令"
3. 把 `examples/` 里的案例作为 Project 知识文件上传（可选,让它诊断更有参照）
4. 之后在这个 Project 里直接开始诊断

---

## 它适合谁

已经在做、卡在某个说不清的地方的一人公司 / 独立开发者 / 小微团队创始人。它不判断"该不该做"（那是早期验证工具的事）,只诊断"已经在跑的业务,为什么卡、怎么破"。

如果你还只有想法、什么都没开始做,它会诚实告诉你:先去做最小验证拿真实信号,再回来诊断。
