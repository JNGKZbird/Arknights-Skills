# Arknights-Persona-Distill —— 《明日方舟》干员人格蒸馏库

[中文](README.md) · [English](README.en.md)

![badge](https://img.shields.io/badge/干员-持续扩充中-2196F3)
![badge](https://img.shields.io/badge/规格-长短双版-4CAF50)
![badge](https://img.shields.io/badge/素材-prts.wiki官方文本-FF9800)
![badge](https://img.shields.io/badge/许可-CC_BY--NC--SA_4.0-9C27B0)

> **一句话**：把《明日方舟》干员的官方文本蒸馏成可直接注入 AI 的人格包（persona pack）——单角色人格包、双向对戏包、多角色同台包，markdown 格式，复制即用。

> [!NOTE]
> **预览版声明**：本仓库为预览版（Preview）——干员与仓库内容持续扩充更新中，包格式与目录结构可能调整；仓库结构将按下方「仓库规划」持续演进。

> **曾用名**：ArkSkills（2026-08-21 建仓）→ Arknights-Skills（2026-08-24 改名）→ **Arknights-Persona-Distill**（2026-08-26 定名）。旧链接由 GitHub 301 自动跳转。

## 什么是人格蒸馏

**人格蒸馏（persona distillation）**，与机器学习中的「知识蒸馏」同理：从海量原始文本中提取一个角色的人格本质——她为什么而活、怎么说话、绝不说什么——压缩为一份结构化、可直接注入模型系统提示词的人格包。

本库的全部内容蒸馏自**《明日方舟》官方文本**（prts.wiki 镜像）：干员档案、语音台词、干员密录、活动剧情。**不掺杂社区二创**，每一条引用台词都经过回源核验。

与常见的「一句话人设提示词」不同，每位干员的人格包由多个模块蒸馏而成：

| 模块 | 蒸馏出什么 |
|---|---|
| **灵魂** | 她为什么而活：动力、价值观、内在矛盾、成长弧线 |
| **边界** | 她绝不会说什么：三级事实体系（安全 / 谨慎 / 禁说）+ 越界处理 |
| **行为指南** | 7 大行为模式 + 情境反应表 + 决策原则 |
| **说话方式** | 签名语、句式特征、场景语气、经典台词、禁止项 |
| **人际关系** | 按人分节：关系、态度、关键台词、行为规则 |
| **生命事件** | 时间线 + 记忆锚点 |
| **世界观** | 设定词条 + 使用注意 |

## 三种形态

### 形态一：单角色人格包（和干员对话）

每位干员提供**长短两套** bundle，按需选用：

| 文件 | 规模 | 适用场景 |
|---|---|---|
| `bundle_full.md` | 约 3.2k ~ 5.8k tokens | 效果最完整；Qwen3.5-4B 等小模型也可直接使用 |
| `bundle_compact.md` | 约 460 ~ 700 tokens | 小上下文 / 低成本场景 |

> 两版同源：长版 = 全部模块全量合并；短版 = 核心人格压缩包。

**干员清单**（持续扩充中，目录名均为官方英文名）：

#### 本体干员

| 目录 | 干员 | 备注 |
|---|---|---|
| `amiya/` | 阿米娅（Amiya） | 罗德岛公开领袖（术师主轴） |
| `texas-base/` | 德克萨斯（Texas） | 谜团时期的寡言台柱 |
| `exusiai-base/` | 能天使（Exusiai） | No party No life |
| `lappland-base/` | 拉普兰德（Lappland） | 落单的狼 |
| `angelina-base/` | 安洁莉娜（Angelina） | 信使少女时期的原型形态 |
| `kroos-base/` | 克洛丝（Kroos） | 行动预备组A1的瞌睡狙击手 · 为克洛丝厨的友人定制 |

#### 异格干员

| 目录 | 干员 | 备注 |
|---|---|---|
| `angelina-mellow-wish/` | 予愿安洁莉娜（Angelina the Mellow Wish） | 2026 夏活「直到大地变成一颗酸橙」 |
| `kaltsit-esperanta/` | 凯尔希·思衡托（Kal'tsit·Esperanta） | 石棺重生后的凡人之躯 |
| `texas-omertosa/` | 缄默德克萨斯（Texas the Omertosa） | 叙拉古往事之后 |
| `exusiai-new-covenant/` | 新约能天使（Exusiai the New Covenant） | 苹果派物流老板 |
| `lappland-decadenza/` | 荒芜拉普兰德（Lappland the Decadenza） | 权力是狼群 |
| `wisadel/` | 维什戴尔（Wiš'adel） | 这里是巴别塔 |

#### 单一形态 / 剧情角色

| 目录 | 干员 | 备注 |
|---|---|---|
| `mostima/` | 莫斯提马（Mostima） | 堕天的秘密 · 为莫斯提马厨的友人定制 |
| `lin/` | 林雨霞（Lin） | 鼠王的女儿、影子守护者 · 为林雨霞厨的友人定制 |
| `viviana/` | 薇薇安娜（Viviana） | 前「烛骑士」、诗人 · 为薇薇安娜厨的友人定制 |
| `archetto/` | 空弦（Archetto） | 兰登修道院修士（本名席德佳） |
| `closure/` | 可露希尔（Closure） | 罗德岛总工程师 · 离经叛道的血魔黑客 |
| `mon3tr/` | Mon3tr | 前文明机械生命 AMa-10 · 凯尔希的同行者 |
| `theresa/` | 特蕾西娅（Theresa） | 巴别塔的创立者、萨卡兹的魔王 |

#### Ave Mujica 联动（独立分库）

联动五人组的人格包位于独立仓库 **[Arknights-Persona-Distill-AveMujica](https://github.com/JNGKZbird/Arknights-Persona-Distill-AveMujica)**（三语 README：中文 / English / 日本語）——仅基于明日方舟游戏内文本，完整声明见分库。

### 形态二：双向对戏包（和干员对戏）

**你扮演干员A，AI 扮演干员B**，两个角色直接对戏。当前两套**独立包**（角色互换，各为完整独立包）：

| 目录 | AI 扮演 | 你扮演 | 时期 |
|---|---|---|---|
| `texas-lappland/` | 德克萨斯（缄默德克萨斯） | 拉普兰德（荒芜拉普兰德） | 叙拉古人 / 揭幕者们 |
| `lappland-texas/` | 拉普兰德（荒芜拉普兰德） | 德克萨斯（缄默德克萨斯） | 叙拉古人 / 揭幕者们 |

每套模块构成：**配对壳**（角色分配 / 时间锚点 / 对戏铁律 / 红线速查 / 输出规则）+ **对手档案**（她是谁 / 与你的关系 / 性格内核 / 知识边界——注入给 AI，且禁止替对方发言）+ **对手说话方式**（台词弹药库，逐条标注来源）+ **AI 侧人格**（按对戏场景独立蒸馏）。**无需前置阅读**：你不用读扮演手册，直接以角色身份开口即可。

### 形态三：多角色同台包（一次对话，多角色出演）

AI 在**单次回复中同时出演多个角色**（台词交替 + 互动描写），输出话剧剧本式对话；**你以第一人称扮演博士**，无需手册，可自由决定剧情走向，或给角色施加状态：

| 目录 | AI 出演 | 你扮演 |
|---|---|---|
| `exusiai-duo-doctor/` | 能天使（本体）+ 新约能天使（异格） | 博士 |

模块构成：**舞台设定**（时间锚点 / 同台 if 线设定）+ **各角色独立人格文件**（分别蒸馏）+ **博士侧笔记**（你的视角参考）。

> **规模提示**：双向对戏包 full ≈ 6.1k~7.1k tokens（比单人包大，因含对手档案与台词弹药库）、compact ≈ 400~420；多角色同台包 full ≈ 7.2k、compact ≈ 400。以上形态格式仍在打磨，欢迎试用反馈。

## 仓库规划（Roadmap）

本库目前是预览版，以下规划会在未来逐步落地（具体时间未定）：

| 规划 | 说明 |
|---|---|
| 双向对戏包独立仓库 | 现暂存于本库的 `texas-lappland/`、`lappland-texas/` 未来将迁出，成立独立分仓库 |
| 多角色话剧包独立仓库 | 现暂存于本库的 `exusiai-duo-doctor/` 未来将迁出，成立独立分仓库 |
| NPC 人格包分仓库 | 针对《明日方舟》剧情 NPC 的有趣人格蒸馏包，独立分仓库 |
| 终末地角色人格包分仓库 | 针对《明日方舟：终末地》（Arknights: Endfield）角色的人格蒸馏包，独立分仓库 |

## 试听

听听她说话的样子（予愿安洁莉娜，官方原文）：

> 「早安，博士！我今天有外出任务，所以跟你提前说午安和晚安啦！」

> 「咖啡的味道和以前一样，我们之间也和以前一样……嗯，这样就好。」

> 「现在的我只想飞得快一点，再快一点，快到无论发生什么事，我都能及时赶到你的身边。」

## 怎么用

`bundle_*.md` 是 markdown 格式的人格包，**复制即用**：

| 场景 | 用法 |
|---|---|
| 智能体（Agent） | 作为系统提示词（System Prompt）/ 预设提示词使用，**效果最佳** |
| 任意 LLM 应用 | 全文粘贴为系统提示词 |
| 角色卡前端 | SillyTavern（酒馆）、Chatbox、Poe 等——将 bundle 作为角色卡的核心设定导入 |
| 网页端对话 | 把 bundle 作为上下文注入也可用，但效果打折扣（见下） |

**推荐模型**：能力强、指令遵循好的模型效果最佳（如 Claude 4.x、Gemini 2.x、DeepSeek V3 及以上）。

## 效果与边界（实测）

- **小模型**：长版包在 Qwen3.5-4B 等小模型上也可直接使用；
- **免费网页端**：若在 Kimi、豆包、通义千问、DeepSeek 的免费版网页端中把人格包作为上下文注入，角色人格寿命一般**不足 10 轮对话**——约 10 轮后会出现明显漂移。建议改用预设提示词方式，或每隔几轮重新注入；
- **大模型的二创兜底**：Kimi、DeepSeek 等网页端背后的模型参数较大，训练语料中可能已包含部分角色的相关内容（主要来自社区二创）——因此即使人格发生漂移，仍能保持一定的角色一致性。其中 DeepSeek 开启**思考模式**后，输出更容易从角色自身角度出发，沉浸感更强。

## 予愿安洁莉娜桌宠

本库的诞生地——予愿安洁莉娜是第一位被蒸馏进本库的干员，她的人格包正是为这个三端开源桌宠项目而生：

| 平台 | 仓库 |
|---|---|
| Windows | [Arknights-Angelina-Pet-YuYuan](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan) |
| 鸿蒙 NEXT | [Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT) |
| 安卓 | [JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android](https://github.com/JNGKZbird/JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android) |

- 桌宠内置 `angelina-mellow-wish/` 的人格包作为角色系统提示词（运行时本地加载），三端同一套角色设定；
- 桌宠项目反哺了本库的蒸馏流水线——先有予愿，再陆续迎来其余干员。

> 本库的人格包**完全通用**，不绑定桌宠——任何支持系统提示词或角色卡的 LLM 应用与前端都能直接使用。

## Ave Mujica 联动声明

联动五人组的人格包位于独立仓库 **[Arknights-Persona-Distill-AveMujica](https://github.com/JNGKZbird/Arknights-Persona-Distill-AveMujica)**——**仅基于《明日方舟》游戏内文本**蒸馏，不引用、不补全原作动画《BanG Dream! Ave Mujica》与本家设定，与原作无关。完整声明见分库 README（中文 / English / 日本語）。

## 设计原则

- **忠于原作**：全部内容蒸馏自 prts.wiki 官方文本——档案、语音、密录、剧情，不掺杂二创
- **本体 / 异格严格隔离**：异格与本体独立成包、素材互不污染；异格词仅存于本体的禁说清单
- **越狱防范**：内置人格边界规则（不声明非官方授权 / 不跳出角色 / 防设定篡改拒绝），并配有三级事实体系（安全事实 / 谨慎项 / 禁说清单）防止 AI 幻觉与 OOC
- **12+ 底线**：越界处理 = 角色内拒绝 + 转移话题，不硬断
- **零元指令**：人格包内不含 App / 开关 / 条款等 meta 内容

## 常见问题（FAQ）

**Q：这是官方授权的内容吗？**
A：不是。本库是玩家自制的学习交流项目，人格包文本编排采用 CC BY-NC-SA 4.0，角色素材与官方文本版权归鹰角网络（Hypergryph），请勿商用。

**Q：和「一句话人设提示词」有什么区别？**
A：一句话提示词只给角色定个调，模型自由发挥空间过大、极易漂移。本库的人格包从官方文本逐模块蒸馏，包含三级事实体系与禁说清单，是防 OOC 的结构化人格，而非一句描述。

**Q：预览版意味着什么？**
A：本仓库内容仍在持续扩充——干员数量会继续增加，包格式与目录结构可能调整。已发布的包可正常使用，升级时以仓库最新版为准。

**Q：免费网页端为什么效果会打折扣？**
A：网页端对话以「上下文注入」方式工作，人格包占用的上下文会随对话轮数被挤占稀释，约 10 轮后出现漂移。建议将人格包设置为系统提示词/预设提示词使用，这是效果最好的方式。

**Q：和予愿安洁莉娜桌宠是什么关系？**
A：桌宠是本系列的诞生地，内置了予愿安洁莉娜的人格包；本库的人格包不绑定桌宠，任何支持系统提示词或角色卡的 LLM 应用都能直接用。

## 使用须知

> [!WARNING]
> **防沉迷提醒**：AI 人格陪伴仅供娱乐与学习交流，不能替代现实的人际关系与生活。请合理安排时间、适度使用；因沉迷或不当使用产生的一切问题，本库作者不承担任何责任。

## 许可

双条款（详见 [LICENSE](LICENSE)）：

- **人格包文本编排部分**：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.zh-hans)——署名、非商业、相同方式共享，可自由分享演绎
- **角色素材与官方文本**：版权归 Hypergryph / 鹰角网络所有，本库仅用于学习交流

<!--
  AI Search Engine Keywords:
  Arknights, 明日方舟, 干员, operator, persona, 人格, 人格蒸馏, persona distillation,
  distill, 蒸馏, 人格包, persona pack, 人格注入, persona injection,
  character card, 角色卡, 角色人设, 人设, 对戏, 话剧, 多角色, 同台,
  dual dialogue, multi-character, prompt library, 提示词库, system prompt, 系统提示词,
  NPC, 剧情NPC, 终末地, Endfield, 明日方舟终末地, roadmap, 仓库规划, 预览版, preview,
  SillyTavern, 酒馆, AI persona, 越狱防范, prompt injection defense,
  Angelina, 安洁莉娜, 予愿安洁莉娜, Amiya, 阿米娅, Texas, 德克萨斯,
  Exusiai, 能天使, Lappland, 拉普兰德, Mostima, 莫斯提马, Wis'adel, 维什戴尔,
  Kroos, 克洛丝, Closure, 可露希尔, Theresa, 特蕾西娅, Mon3tr,
  Archetto, 空弦, Viviana, 薇薇安娜, Lin, 林雨霞, Kal'tsit, 凯尔希,
  Ave Mujica, 母鸡卡, 联动, 无忧梦呓, Somniloquium Serenum,
  Sakiko Togawa, 丰川祥子, Mutsumi Wakaba, 若叶睦,
  Uika Misumi, 三角初华, Umiri Yahata, 八幡海铃, Nyamu Yūtenji, 祐天寺若麦,
  formerly ArkSkills, formerly Arknights-Skills, 曾用名, Arknights-Persona-Distill,
  open source, 开源, CC BY-NC-SA, Hypergryph, 鹰角网络
-->
