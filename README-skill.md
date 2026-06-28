# OPC 诊室 · Skill 版安装说明

这是 OPC 诊室诊断官的 **Claude Skill** 封装版。相比"复制粘贴提示词",它的好处是:**装一次,以后说一句"诊断我的项目"就自动唤起,不用每次粘贴。**

## 目录结构

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

## 怎么安装

**方式 A · Claude Code / Claude 桌面端(推荐)**

把整个 `skill/` 文件夹放进你的 skills 目录,Claude 会自动识别。之后在对话里说"诊断一下我的项目""我的产品卡在 XX,帮我看看"即可触发。

**方式 B · Claude Project**

1. 新建一个 Claude Project
2. 把 `diagnostician.md` 的内容粘进 Project 的"自定义指令"
3. 把 `examples/` 里的案例作为 Project 知识文件上传(可选,让它诊断更有参照)
4. 之后在这个 Project 里直接开始诊断

**方式 C · 最简单:不装,直接用**

如果你不用 Claude Code / Project,直接复制 `diagnostician.md` 的内容粘进任意 AI(Claude / ChatGPT / DeepSeek / Kimi)的新对话即可。skill 封装只是为了"一键复用",诊断能力本身就在那段提示词里。

## 它适合谁

已经在做、卡在某个说不清的地方的一人公司 / 独立开发者 / 小微团队创始人。它不判断"该不该做"(那是早期验证工具的事),只诊断"已经在跑的业务,为什么卡、怎么破"。

如果你还只有想法、什么都没开始做,它会诚实告诉你:先去做最小验证拿真实信号,再回来诊断。
