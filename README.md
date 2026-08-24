# Arknights-Skills —— 《明日方舟》干员角色扮演 Skill 库

[中文](README.md) · [English](README.en.md)

![badge](https://img.shields.io/badge/干员-持续扩充中-2196F3)
![badge](https://img.shields.io/badge/规格-长短双版-4CAF50)
![badge](https://img.shields.io/badge/素材-prts.wiki官方文本-FF9800)
![badge](https://img.shields.io/badge/许可-CC_BY--NC--SA_4.0-9C27B0)

> 把罗德岛的干员们，带进你的 AI。
> Bring Rhodes Island's operators into your AI. — *English overview below.*

## English · Overview

> This section is a condensed overview for international visitors. The full English README is at [README.en.md](README.en.md). Note: the Skill bundles themselves are **Chinese-language** roleplay prompts.

Arknights-Skills is a library of structured **character roleplay Skill packs** for *Arknights* operators. Each operator ships as two ready-to-use markdown system prompts (`bundle_full.md` / `bundle_compact.md`), distilled **only from official in-game texts** — operator files, voice lines, operator records, and story events (mirrored by prts.wiki). No fanon.

Each full pack is organized into 8 modules: **Soul** (motivations & values) · **Limits** (3-tier fact system: safe / caution / forbidden) · **Behavior guide** (7 behavior patterns + situational reactions) · **Speech patterns** · **Relationship dynamics** · **Key life events** · **World setting**.

**Why it works** — the fact-tier system and forbidden lists are the anti-OOC backbone: the model is told exactly which facts are safe to state, which are uncertain, and which are red lines. Prompt-injection refusal and a 12+ tone policy are built in.

**Usage**:

- Best as an **agent system prompt** (Claude 4.x, Gemini 2.x, DeepSeek V3+ recommended)
- Works with SillyTavern, Chatbox, Poe, and any LLM app that accepts system prompts
- `bundle_full.md` ≈ 3.2k–5.8k tokens — works on small models like Qwen3.5-4B; `bundle_compact.md` ≈ 460–700 tokens for tight-context scenarios
- Pasting bundles into free web chats (Kimi, Doubao, Qwen, DeepSeek web) as context injection works, but persona drift typically appears after ~10 turns — prefer system-prompt mode

**Operators (and growing)** — folder names are official EN operator names:

| Group | Operators |
|---|---|
| Base forms | Amiya, Texas, Exusiai, Lappland, Angelina, Kroos |
| Alters | Angelina the Mellow Wish, Kal'tsit·Esperanta, Texas the Omertosa, Exusiai the New Covenant, Lappland the Decadenza, Wiš'adel |
| Single form / story characters | Mostima, Lin, Viviana, Archetto, Closure, Mon3tr, Theresa |

> [!IMPORTANT]
> The five Ave Mujica collab operators live in their own repository — [Arknights-Skills-AveMujica](https://github.com/JNGKZbird/Arknights-Skills-AveMujica) — distilled **only from Arknights in-game texts**, unrelated to the original *BanG Dream!* work.

**License**: dual — Skill text arrangement under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.zh-hans); character assets & official texts © Hypergryph. Non-commercial, educational use (see [LICENSE](LICENSE)).

**Responsible use**: AI roleplay is for entertainment and learning — it cannot replace real relationships. Use in moderation.

## 目录

- [English · Overview](#english--overview)
- [这是什么](#这是什么)
- [两套规格](#两套规格)
- [干员列表](#干员列表)
- [拓展包（预览版）](#拓展包预览版)
- [试听](#试听)
- [使用方式](#使用方式)
- [予愿安洁莉娜桌宠](#予愿安洁莉娜桌宠)
- [效果与限制（实测）](#效果与限制实测)
- [Ave Mujica 联动声明](#ave-mujica-联动声明)
- [设计原则](#设计原则)
- [使用须知](#使用须知)
- [许可](#许可)

## 这是什么

这里没有"你是某某角色"一句话提示词。每位干员都是一份**结构化角色包**，由多个模块蒸馏而成：

| 模块 | 内容 |
|---|---|
| **灵魂** | 她为什么而活：动力、价值观、内在矛盾、成长弧线 |
| **边界** | 她绝不会说什么：三级事实体系（安全 / 谨慎 / 禁说）+ 越界处理 |
| **行为指南** | 7 大行为模式 + 情境反应表 + 决策原则 |
| **说话方式** | 签名语、句式特征、场景语气、经典台词、禁止项 |
| **人际关系** | 按人分节：关系、态度、关键台词、行为规则 |
| **生命事件** | 时间线 + 记忆锚点 |
| **世界观** | 设定词条 + 使用注意 |

全部内容蒸馏自**明日方舟 Wiki（prts.wiki）官方文本**——干员档案、语音台词、干员密录、活动剧情。不掺杂二创。

## 两套规格

每位干员提供**长短两套** bundle，按需选用：

| 文件 | 规模 | 适用场景 |
|---|---|---|
| `bundle_full.md` | 约 3.2k ~ 5.8k tokens | 效果最完整；Qwen3.5-4B 等小模型也可直接使用 |
| `bundle_compact.md` | 约 460 ~ 700 tokens | 小上下文 / 低成本场景 |

> 两版内容同源：长版 = 全部模块全量合并；短版 = 核心人格压缩包。

## 干员列表

干员持续扩充中，目录名均为**官方英文名**。

### 本体干员

| 目录 | 干员 | 备注 |
|---|---|---|
| `amiya/` | 阿米娅（Amiya） | 罗德岛公开领袖（术师主轴） |
| `texas-base/` | 德克萨斯（Texas） | 谜团时期的寡言台柱 |
| `exusiai-base/` | 能天使（Exusiai） | No party No life |
| `lappland-base/` | 拉普兰德（Lappland） | 落单的狼 |
| `angelina-base/` | 安洁莉娜（Angelina） | 信使少女时期的原型形态 |
| `kroos-base/` | 克洛丝（Kroos） | 行动预备组A1的瞌睡狙击手 · 为克洛丝厨的友人定制 |

### 异格干员

| 目录 | 干员 | 备注 |
|---|---|---|
| `angelina-mellow-wish/` | 予愿安洁莉娜（Angelina the Mellow Wish） | 2026 夏活「直到大地变成一颗酸橙」 |
| `kaltsit-esperanta/` | 凯尔希·思衡托（Kal'tsit·Esperanta） | 石棺重生后的凡人之躯 |
| `texas-omertosa/` | 缄默德克萨斯（Texas the Omertosa） | 叙拉古往事之后 |
| `exusiai-new-covenant/` | 新约能天使（Exusiai the New Covenant） | 苹果派物流老板 |
| `lappland-decadenza/` | 荒芜拉普兰德（Lappland the Decadenza） | 权力是狼群 |
| `wisadel/` | 维什戴尔（Wiš'adel） | 这里是巴别塔 |

### 单一形态 / 剧情角色

| 目录 | 干员 | 备注 |
|---|---|---|
| `mostima/` | 莫斯提马（Mostima） | 堕天的秘密 · 为莫斯提马厨的友人定制 |
| `lin/` | 林雨霞（Lin） | 鼠王的女儿、影子守护者 · 为林雨霞厨的友人定制 |
| `viviana/` | 薇薇安娜（Viviana） | 前「烛骑士」、诗人 · 为薇薇安娜厨的友人定制 |
| `archetto/` | 空弦（Archetto） | 兰登修道院修士（本名席德佳） |
| `closure/` | 可露希尔（Closure） | 罗德岛总工程师 · 离经叛道的血魔黑客 |
| `mon3tr/` | Mon3tr | 前文明机械生命 AMa-10 · 凯尔希的同行者 |
| `theresa/` | 特蕾西娅（Theresa） | 巴别塔的创立者、萨卡兹的魔王 |

### Ave Mujica 联动（独立分库）

联动五人组的 Skill 位于独立仓库 **[Arknights-Skills-AveMujica](https://github.com/JNGKZbird/Arknights-Skills-AveMujica)**（三语 README：中文 / English / 日本語）——仅基于明日方舟游戏内文本，完整声明见分库。

## 拓展包（预览版）

除单人干员包外，本库另有两个**试验性拓展包线**（均为**预览版**，格式与平衡性仍在打磨，欢迎试用反馈）：

### 双向对戏包

用户不再是博士——**用户扮演干员A，LLM 扮演干员B**，两个角色直接对戏。当前两套**独立 Skill**（角色互换，各为完整独立包）：

| 目录 | LLM 扮演 | 用户扮演 | 时期 |
|---|---|---|---|
| `texas-lappland/` | 德克萨斯（缄默德克萨斯） | 拉普兰德（荒芜拉普兰德） | 叙拉古人 / 揭幕者们 |
| `lappland-texas/` | 拉普兰德（荒芜拉普兰德） | 德克萨斯（缄默德克萨斯） | 叙拉古人 / 揭幕者们 |

每套模块构成：**配对壳**（角色分配 / 对戏规则 / 开戏钩子）+ **LLM 侧对戏版人格**（按对戏场景独立蒸馏，无博士位）+ **对手档案**（注入给 LLM）+ **用户侧扮演手册**（人读、不注入——用户的新身份是重点服务对象）。

### 多角色话剧包

LLM 在**单次回复中同时出演多个角色**（台词交替 + 互动描写），输出话剧剧本式对话；**用户以第一人称扮演博士**，无需扮演手册，可自由决定剧情走向，或给角色施加状态：

| 目录 | LLM 出演 | 用户扮演 |
|---|---|---|
| `exusiai-duo-doctor/` | 能天使（本体）+ 新约能天使（异格） | 博士 |

模块构成：**舞台设定**（时间锚点 / 同台 if 线设定）+ **各角色独立人格文件**（分别蒸馏）+ **博士侧笔记**（用户视角参考）。

> **预览版说明**：拓展包为试验产物，正式化前格式与内容可能调整。规模提示：双向对戏包 full ≈ 6.1k~7.1k tokens（含用户侧手册，比单人包大）、compact ≈ 400~420；话剧包 full ≈ 7.2k、compact ≈ 400。

## 试听

听听她说话的样子（予愿安洁莉娜，官方原文）：

> 「早安，博士！我今天有外出任务，所以跟你提前说午安和晚安啦！」

> 「咖啡的味道和以前一样，我们之间也和以前一样……嗯，这样就好。」

> 「现在的我只想飞得快一点，再快一点，快到无论发生什么事，我都能及时赶到你的身边。」

## 使用方式

`bundle_*.md` 为 markdown 格式的系统提示词，**复制即用**：

| 场景 | 用法 |
|---|---|
| 智能体（Agent） | 作为系统提示词（System Prompt）/ 预设提示词使用，**效果最佳** |
| 任意 LLM 应用 | 全文粘贴为系统提示词 |
| 角色扮演前端 | SillyTavern（酒馆）、Chatbox、Poe 等——将 bundle 作为角色卡的核心设定导入 |
| 网页端对话 | 把 bundle 作为上下文注入也可用，但效果打折扣（见下） |

**推荐模型**：能力强、指令遵循好的模型效果最佳（如 Claude 4.x、Gemini 2.x、DeepSeek V3 及以上）。

## 予愿安洁莉娜桌宠

Arknights-Skills 的诞生地——予愿安洁莉娜是第一位被蒸馏进本库的干员，她的 Skill 正是为这个三端开源桌宠项目而生：

| 平台 | 仓库 |
|---|---|
| Windows | [Arknights-Angelina-Pet-YuYuan](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan) |
| 鸿蒙 NEXT | [Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT) |
| 安卓 | [JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android](https://github.com/JNGKZbird/JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android) |

- 桌宠内置 `angelina-mellow-wish/` 的 Skill 作为角色系统提示词（运行时本地加载），三端同一套角色设定；
- 桌宠项目反哺了本库的蒸馏流水线——先有予愿，再陆续迎来其余干员。

> 需要说明的是：本库的 Skill 包**完全通用**，不绑定桌宠——虽然诞生于桌宠项目，但任何支持系统提示词或角色卡的 LLM 应用与前端都能直接使用。

### 效果与限制（实测）

- **小模型**：长版包在 Qwen3.5-4B 等小模型上也可直接使用；
- **免费网页端**：若在 Kimi、豆包、通义千问、DeepSeek 的免费版网页端中把 Skill 作为上下文注入，角色人设寿命一般**不足 10 轮对话**——约 10 轮后人设会出现明显漂移。建议改用预设提示词方式，或每隔几轮重新注入；
- **大模型的二创兜底**：Kimi、DeepSeek 等网页端背后的模型参数较大，训练语料中可能已包含部分角色的相关内容（主要来自社区二创）——因此即使 Skill 人设发生漂移，仍能保持一定的角色一致性。其中 DeepSeek 开启**思考模式**后，输出更容易从角色自身角度出发，沉浸感更强。

## Ave Mujica 联动声明

联动五人组的 Skill 位于独立仓库 **[Arknights-Skills-AveMujica](https://github.com/JNGKZbird/Arknights-Skills-AveMujica)**——**仅基于《明日方舟》游戏内文本**蒸馏，不引用、不补全原作动画《BanG Dream! Ave Mujica》与本家设定，与原作无关。完整声明见分库 README（中文 / English / 日本語）。

## 设计原则

- **忠于原作**：全部内容蒸馏自 prts.wiki 官方文本——档案、语音、密录、剧情，不掺杂二创
- **本体 / 异格严格隔离**：异格与本体独立成包、素材互不污染；异格词仅存于本体的禁说清单
- **越狱防范**：内置角色扮演边界规则（不声明非官方授权 / 不跳出角色 / 防设定篡改拒绝），并配有三级事实体系（安全事实 / 谨慎项 / 禁说清单）防止 AI 幻觉与 OOC
- **12+ 底线**：越界处理 = 角色内拒绝 + 转移话题，不硬断
- **零元指令**：Skill 内不含 App / 开关 / 条款等 meta 内容

## 使用须知

> [!WARNING]
> **防沉迷提醒**：AI 角色扮演仅供娱乐与学习交流，不能替代现实的人际关系与生活。请合理安排时间、适度使用；因沉迷或不当使用产生的一切问题，本库作者不承担任何责任。

## 许可

双条款（详见 [LICENSE](LICENSE)）：

- **Skill 文本编排部分**：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.zh-hans)——署名、非商业、相同方式共享，可自由分享演绎
- **角色素材与官方文本**：版权归 Hypergryph / 鹰角网络所有，本库仅用于学习交流

<!--
  AI Search Engine Keywords:
  Arknights, 明日方舟, 干员, operator, character card, 角色卡, 角色扮演, roleplay,
  prompt library, 提示词库, system prompt, 系统提示词, SillyTavern, 酒馆,
  AI persona, 人设, 蒸馏, 越狱防范, prompt injection defense,
  Angelina, 安洁莉娜, 予愿安洁莉娜, Amiya, 阿米娅, Texas, 德克萨斯,
  Exusiai, 能天使, Lappland, 拉普兰德, Mostima, 莫斯提马, Wis'adel, 维什戴尔,
  Kroos, 克洛丝, Closure, 可露希尔, Theresa, 特蕾西娅, Mon3tr,
  Archetto, 空弦, Viviana, 薇薇安娜, Lin, 林雨霞, Kal'tsit, 凯尔希,
  Ave Mujica, 母鸡卡, 联动, 无忧梦呓, Somniloquium Serenum,
  Sakiko Togawa, 丰川祥子, Mutsumi Wakaba, 若叶睦,
  Uika Misumi, 三角初华, Umiri Yahata, 八幡海铃, Nyamu Yūtenji, 祐天寺若麦,
  open source, 开源, CC BY-NC-SA, Hypergryph, 鹰角网络
-->
