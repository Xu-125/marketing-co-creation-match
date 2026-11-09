# 我能为你做什么 · What Can We Do for You?

**English:** An Agent Skill for finding a practical collaboration starting point by matching your resources with a partner's needs.

[中文说明](#你会拿到什么) · [English guide](#english-guide)

给做产品营销、PR、品牌和客户合作的人用的 Skill。任何支持读取 Skill 指令的 Agent 都可以用，只要它能通过 CLI 或检索工具读取你的背景。你说一个要对接的对象，它帮你查背景、找需求，再想清楚可以一起做什么。

搜过对方的采访，也看过自家产品介绍，还是不知道该从哪里谈起？这个 Skill 会把两边放在一起看：对方正在做什么，你这边有哪些资源、合作进展和产品能力。

## 你会拿到什么

- **一个合作切入点**：先帮对方哪件事，理由是什么。
- **一个共创方向**：谁参与、怎么玩、对方能拿到什么，公众为什么愿意看。
- **需要确认的条件**：只写会影响方向的缺口，不把猜测写成事实。

已有合作在推进时，它查当前进展和卡点；产业客户资料少时，它结合公司、岗位和沟通片段提出待验证的方向。不要求先填需求表，也不生成一套访谈问卷。

## 看一个例子

> 我是产品营销人员，能组织内容制作。对方是制造企业的市场负责人，说“新品技术亮点很多，渠道还是讲不清”。我们能帮什么？

**输出示意｜把一个卖点讲明白**

先从一个难解释的卖点入手，做“一页解释 + 一个演示场景”。你组织技术专家和渠道同事，产品整理技术资料、写讲解草稿，内容团队完成演示。让技术差异出现在具体使用场景里，渠道能讲，客户能懂。

这是虚构场景的方向演示，不是已落地案例。更多输入输出对照见 [示例](marketing-co-creation-match/references/examples.md)。

## 它会查哪些背景

一边查用户：身份、能协调的资源、内部讨论、立项材料、合作进度和产品实际能力。另一边查对方：当前身份、近期项目、公开表述；客户则结合公司、岗位与已有跟进。

查你的背景是核心步骤。来源可以是 CLI 能读取的项目文件、个人笔记，也可以是获授权检索的群聊、文档、邮件或客户跟进。它不会只搜对方，也不会把一张产品功能清单当成你的全部能力。不绑定某个平台、模型或专属工具，安装后仍只能使用你已授权的资料。

## 安装与试用

这是一个文件型 Skill，没有额外的软件包和 API Key。

1. 下载或克隆本仓库。
2. 在支持 Agent Skills 的工具中，按其安装方式导入 `marketing-co-creation-match/` 整个文件夹。保留 `SKILL.md` 与 `references/` 的相对位置，别只复制单个文件。
3. 确认 Agent 能通过 CLI 或检索工具读取你的背景，并能查询对方的相关资料，再用一句真实需求试跑。

也可以让你的 Agent 从本仓库安装 `marketing-co-creation-match/`。不同客户端的安装入口不同，请按客户端支持的方式操作。

```text
我要对接【姓名 / 公司与岗位】，我们能为他做什么？
```

有一句客户原话或项目材料，顺手附上即可：

```text
对方是【公司与岗位】，他提到【原话】。
结合我们这边的背景，给我一个合作切入点和共创方向。
```

## 使用条件

- **Agent**：能读取 Skill 指令，并使用 CLI 或检索工具获取资料即可，不要求特定产品、模型、企业连接器或工具名称。
- **背景来源**：可用本地项目、个人笔记、知识库或已授权的业务资料。Agent 按当前环境选择读取方式；没有访问能力时，只能基于你提供的材料给有限建议，不能声称已查过。
- **对方资料**：通过已有公开检索工具、CLI 或你提供的材料获取；查不到的事实明确标注，不用常识补成事实。
- **隐私**：不要把内部聊天、客户资料、报价或凭据提交到本公开仓库。本仓库只包含通用指令与虚构示例，不含企业内部材料。

## 文件与验证范围

`README.md` 是介绍；`marketing-co-creation-match/SKILL.md` 是执行规则；`references/examples.md` 是输出参考。Skill 目录不含脚本，没有自动发布、联系合作方或支付功能。

当前为首版：已做文件结构、元数据、引用路径和公开内容检查。尚未完成独立会话中的触发测试与有/无 Skill 对照测试，不承诺安装后在所有客户端都能自动调用工具。

拿下一位要对接的人试一次：看看它有没有找到你漏掉的背景，推荐是否贴合对方，玩法是否值得继续聊。反馈可以提 Issue，请使用脱敏或虚构输入。

---

## English guide

### What Can We Do for You?

An Agent Skill for product marketing, PR, brand, and customer-partnership work. Name the person or customer you want to work with, and it helps research both sides, identify a useful starting point, and suggest something worth doing together.

It is for the moment when you have read the partner's interviews and your own product materials but still do not know where to begin. It considers what the partner is working on alongside your resources, existing cooperation, and verified product capabilities.

### What you get

- **A collaboration starting point:** what to help the partner with first, and why.
- **A co-creation direction:** who participates, how it works, what the partner gains, and why an audience would care.
- **Conditions to confirm:** only the missing information that could change the direction; guesses are not presented as facts.

For an ongoing partnership, the Skill focuses on current progress and blockers. For a customer with limited documentation, it uses the company, role, and available conversation excerpts to suggest a direction that still needs validation. It does not require a needs form or produce an interview questionnaire by default.

### A fictional example

> I work in product marketing and can coordinate content production. The marketing lead at a manufacturing company says, “Our new product has plenty of technical strengths, but our channel partners still cannot explain them clearly.” What can we help with?

**Suggested direction — Make one selling point clear**

Start with one difficult-to-explain feature and create a one-page explanation plus a demonstration scenario. You coordinate technical experts and channel colleagues; the product helps organize technical materials and draft the explanation; the content team produces the demonstration. Show the technical difference in a concrete use case so channel partners can explain it and customers can understand it.

This is an illustration, not a completed partnership or a verified product test. See [more fictional examples](marketing-co-creation-match/references/examples.md#english-examples).

### What background it checks

**Your side:** your role, goals, resources you can coordinate, authorized project files and notes, internal discussions, proposal materials, partnership progress, and relevant product capabilities.

**The partner's side:** current role, recent work, and public statements. For customers, it also considers the company, job responsibilities, and existing follow-up records.

Researching your background is a core step—not just reading a product feature list. Sources may include local files accessible through CLI, personal notes, or authorized chat, document, email, and customer-record searches. The Skill is not tied to a platform, model, or proprietary tool and never grants access beyond your existing permissions.

### Install and try

This is a file-based Skill, with no additional software package or API key supplied by the Skill itself.

1. Download or clone this repository.
2. Import the entire `marketing-co-creation-match/` folder into a tool that supports Agent Skills, following that tool's installation procedure. Keep `SKILL.md` and `references/` in their relative locations.
3. Check that the agent can access your background through authorized CLI or search tools and can research the partner. Try one real request.

You can also ask your agent to install `marketing-co-creation-match/` from this repository. Installation entry points vary by client.

```text
I want to work with [name / company and role]. What can we do for them?
```

If you have a customer quote or project material, include it:

```text
The partner is [company and role], and they said [exact quote].
Use our background to suggest a collaboration starting point and a co-creation direction.
```

### Requirements and privacy

- **Agent:** must read Skill instructions and use available CLI or search tools. No particular product, model, enterprise connector, or tool name is required.
- **Your background:** may come from local projects, notes, knowledge bases, or authorized business materials. Without access, the agent must limit its advice to supplied material and must not claim to have researched inaccessible sources.
- **Partner information:** obtain it through available public search, CLI, or supplied materials. Mark missing facts rather than filling them in with assumptions.
- **Privacy:** never commit internal chats, customer data, quotations, pricing, or credentials to this public repository. It contains generic instructions and fictional examples only.

### Files and validation status

`README.md` introduces the Skill. [`marketing-co-creation-match/SKILL.md`](marketing-co-creation-match/SKILL.md#english-instructions) contains execution rules. `references/examples.md` illustrates the output style. The Skill folder has no scripts and does not automatically publish content, contact partners, or make payments.

This is the first version. File structure, metadata, reference paths, and public-content checks have been performed. Independent-session trigger tests and with/without-Skill comparison tests have not yet been completed. Automatic tool invocation across all clients is not guaranteed.

Try it with the next person you want to approach. Check whether it finds background you missed, whether the recommendation fits the partner, and whether the proposed format is worth discussing. Issues are welcome; use anonymized or fictional inputs.
