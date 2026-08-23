# ArkSkills —— 《明日方舟》干员角色扮演 Skill 库

![badge](https://img.shields.io/badge/干员-24位-2196F3)
![badge](https://img.shields.io/badge/格式-Markdown-4CAF50)
![badge](https://img.shields.io/badge/素材-明日方舟Wiki官方文本-FF9800)
![badge](https://img.shields.io/badge/许可-素材归鹰角网络-9C27B0)

把罗德岛的干员们，带进你的 AI。

这里没有粗糙的"你是某某角色"一句话提示词——每一位干员都是一份**结构化角色包**：灵魂（她为什么而活）、边界（她绝不会说什么）、行为指南（七大行为模式 + 情境反应表）、说话方式（签名语、句式特征、官方原文示例），全部蒸馏自**明日方舟 Wiki 官方文本**。

> 听听她说话的样子（予愿安洁莉娜，官方原文）：

> 「早安，博士！我今天有外出任务，所以跟你提前说午安和晚安啦！」
> 「咖啡的味道和以前一样，我们之间也和以前一样……嗯，这样就好。」
> 「现在的我只想飞得快一点，再快一点，快到无论发生什么事，我都能及时赶到你的身边。」

## 两套规格

每位干员提供**长短两套**，按需选用：

| 文件 | 用途 |
|---|---|
| `bundle_compact.md` | **短版**：核心人格压缩包，适合小上下文 / 低成本场景 |
| `bundle_full.md` | **完整长版**：灵魂 / 边界 / 行为指南 / 说话方式全量合并，效果最完整；Qwen3.5-4B 等小模型也可直接使用 |

## 干员列表

| 目录 | 干员 | 备注 |
|---|---|---|
| `angelina-mellow-wish/` | 予愿安洁莉娜（Angelina the Mellow Wish） | 2026 夏活「直到大地变成一颗酸橙」，信使少女 |
| `angelina-base/` | 安洁莉娜（本体） | 信使少女时期的原型形态 |
| `amiya/` | 阿米娅 | 罗德岛公开领袖（术师主轴） |
| `kaltsit-esperanta/` | 凯尔希·思衡托（Kal'tsit·Esperanta） | 石棺重生后的凡人之躯（异格） |
| `texas-base/` | 德克萨斯（本体） | 谜团时期的寡言台柱 |
| `texas-omertosa/` | 缄默德克萨斯 | 叙拉古往事之后 |
| `exusiai-base/` | 能天使（本体） | No party No life |
| `exusiai-new-covenant/` | 新约能天使（Exusiai the New Covenant） | 苹果派物流老板 |
| `lappland-base/` | 拉普兰德（本体） | 落单的狼 |
| `lappland-decadenza/` | 荒芜拉普兰德 | 权力是狼群 |
| `lin/` | 林雨霞（Lin） | 鼠王的女儿、影子守护者 · 为林雨霞厨的友人定制 |
| `mostima/` | 莫斯提马 | 堕天的秘密 · 为莫斯提马厨的友人定制 |
| `wisadel/` | 维什戴尔 | 这里是巴别塔 |
| `kroos-base/` | 克洛丝（本体） | 行动预备组A1的瞌睡狙击手 · 为克洛丝厨的友人定制 |
| `closure/` | 可露希尔 | 罗德岛总工程师 · 离经叛道的血魔黑客 |
| `theresa/` | 特蕾西娅 | 巴别塔的创立者、萨卡兹的魔王 |
| `mon3tr/` | Mon3tr | 前文明机械生命 AMa-10 · 凯尔希的同行者 |
| `archetto/` | 空弦 | 兰登修道院修士（本名席德佳） |
| `viviana/` | 薇薇安娜 | 前「烛骑士」、诗人 · 为薇薇安娜厨的友人定制 |
| `togawa-sakiko/` | 丰川祥子（Togawa Sakiko） | Ave Mujica 联动 · 键盘手（Oblivionis） |
| `wakaba-mutsumi/` | 若叶睦（Wakaba Mutsumi） | Ave Mujica 联动 · 吉他手（Mortis） |
| `misumi-uika/` | 三角初华（Misumi Uika） | Ave Mujica 联动 · 主唱兼吉他手（Doloris） |
| `yahata-umiri/` | 八幡海铃（Yahata Umiri） | Ave Mujica 联动 · 贝斯手（Timoris） |
| `yutenji-nyamu/` | 祐天寺若麦（Yūtenji Nyamu） | Ave Mujica 联动 · 鼓手（Amoris） |

## 关于 Ave Mujica 联动干员（重要声明）

本库中丰川祥子、若叶睦、三角初华、八幡海铃、祐天寺若麦五位干员的 Skill，**仅基于《明日方舟》游戏内文本**蒸馏——包括干员档案、语音台词与联动 SideStory「无忧梦呓」（Somniloquium Serenum）的登场剧情。

- **不引用、不补全**原作动画《BanG Dream! Ave Mujica》及 BanG Dream! 本家企划的任何设定与剧情；
- 原作中官方留白的内容（如角色关系走向、个人经历细节），在 Skill 中同样**保持留白**；
- 这些 Skill 与原作动画无关，不构成对原作的演绎或续写。

## 使用方式

`bundle_*.md` 为 markdown 格式的系统提示词，**复制即用**：

- **智能体（Agent）预设提示词**：本库 Skill 最适合作为智能体的系统提示词（System Prompt）使用，效果最佳
- **任意 LLM 应用**：全文粘贴为系统提示词（System Prompt）
- **网页端上下文注入**：在网页对话中直接把 bundle 作为上下文注入也可用，但效果会打折扣——人设维持时间与稳定性不如预设提示词方式
- **角色扮演前端**：兼容 SillyTavern（酒馆）、Chatbox、Poe 等——将 bundle 内容作为角色卡的核心设定导入
- **予愿安洁莉娜桌宠**（三端开源，内置本库 Skill 的运行时加载）：
  - Windows：[Arknights-Angelina-Pet-YuYuan](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan)
  - 鸿蒙：[Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT)
  - 安卓：[JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android](https://github.com/JNGKZbird/JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android)

**效果提示（实测经验）**：

- 长版包在 Qwen3.5-4B 等小模型上也可直接使用；
- 若在 Kimi、豆包、通义千问、DeepSeek 的**免费版网页端**中把 Skill 作为上下文注入，角色人设寿命一般**不足 10 轮对话**——约 10 轮后人设会出现明显漂移。建议改用预设提示词方式，或每隔几轮重新注入；
- Kimi、DeepSeek 等网页端背后的模型参数较大，训练语料中可能已包含部分角色的相关内容（主要来自社区二创）——因此即使 Skill 人设发生漂移，仍能保持一定的角色一致性。其中 DeepSeek 开启**思考模式**后，输出更容易从角色自身角度出发，沉浸感更强。

## 使用须知（免责声明）

- **防沉迷提醒**：AI 角色扮演仅供娱乐与学习交流，不能替代现实的人际关系与生活。请合理安排时间、适度使用；因沉迷或不当使用产生的一切问题，本库作者不承担任何责任。

**推荐模型**：能力强、指令遵循好的模型效果最佳（如 Claude 4.x、Gemini 2.x、DeepSeek V3 及以上）。

## 关于这些 Skill

- **忠于原作**：全部内容蒸馏自明日方舟 Wiki（prts.wiki）官方文本——干员档案、语音台词、密录、活动剧情。不掺杂二创。
- **越狱防范**：每个 Skill 内置角色扮演边界规则（"不声明非官方授权""不跳出角色""防设定篡改拒绝"），并配有三级事实体系（安全事实 / 谨慎项 / 禁说清单）防止 AI 幻觉与 OOC。
- **角色统一性**：异格与本体独立成包、素材严格隔离，异格词仅存于本体的禁说清单。

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
  Archetto, 空弦, Viviana, 薇薇安娜,
  Ave Mujica, 母鸡卡, 联动, 无忧梦呓, Somniloquium Serenum,
  Sakiko Togawa, 丰川祥子, Mutsumi Wakaba, 若叶睦,
  Uika Misumi, 三角初华, Umiri Yahata, 八幡海铃, Nyamu Yūtenji, 祐天寺若麦,
  open source, 开源, CC BY-NC-SA, Hypergryph, 鹰角网络
-->
