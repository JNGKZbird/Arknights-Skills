# Arknights-Persona-Distill — Operator Persona Distillation Library for *Arknights*, from Official Texts

[English](README.en.md) · [中文](README.md)

![badge](https://img.shields.io/badge/Operators-growing-2196F3)
![badge](https://img.shields.io/badge/Format-Markdown-4CAF50)
![badge](https://img.shields.io/badge/Source-prts.wiki_official_texts-FF9800)
![badge](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-9C27B0)

> **In one sentence**: persona packs for *Arknights* operators, distilled from official in-game texts and ready to inject into any AI — solo packs, duet packs, and multi-character stage packs, in markdown. Copy and use.

> [!NOTE]
> **Preview notice**: this repository is in preview — operators and content keep growing and updating; pack formats and directory layout may change.

> **Former names**: ArkSkills (created 2026-08-21) → Arknights-Skills (renamed 2026-08-24) → **Arknights-Persona-Distill** (2026-08-26). Old links 301-redirect automatically.

## What Is Persona Distillation

**Persona distillation** — analogous to *knowledge distillation* in machine learning: extract the essence of a character's persona from a large corpus of raw texts — what she lives for, how she speaks, what she would never say — and compress it into a structured pack that can be injected directly as a model's system prompt.

Everything in this library is distilled **only from official *Arknights* texts** (mirrored by prts.wiki): operator files, voice lines, operator records, and story events. **No community fanon**; every quoted line is verified against its source.

Unlike the common "you are character X" one-liner, each operator's persona pack is distilled into modules:

| Module | What it distills |
|---|---|
| **Soul** | What she lives for: drives, values, inner conflicts, growth arc |
| **Limits** | What she would never say: a 3-tier fact system (safe / caution / forbidden) + boundary handling |
| **Behavior Guide** | 7 behavior patterns + situational if-then reactions + decision principles |
| **Speech Patterns** | Signature phrases, sentence habits, scene-specific tones, iconic lines, bans |
| **Relationship Dynamics** | Per-person sections: relation, attitude, key lines, behavior rules |
| **Key Life Events** | Timeline + memory anchors |
| **World Setting** | Lore entries + usage cautions |

## Three Forms

### Form 1: Solo Persona Packs (chat with an operator)

Each operator ships two bundles:

| File | Size | Use When |
|---|---|---|
| `bundle_full.md` | ≈ 3.2k – 5.8k tokens | Fullest effect; works on small models like Qwen3.5-4B |
| `bundle_compact.md` | ≈ 460 – 700 tokens | Tight-context / low-cost scenarios |

> Same source material: full = all modules merged; compact = core-persona compression.

**Operator list** (growing; folder names are official EN operator names):

#### Base Forms

| Folder | Operator | Notes |
|---|---|---|
| `amiya/` | Amiya | Rhodes Island's public leader (Caster-focused) |
| `texas-base/` | Texas | The taciturn ace of her mysterious early days |
| `exusiai-base/` | Exusiai | No party No life |
| `lappland-base/` | Lappland | The lone wolf |
| `angelina-base/` | Angelina | Her original messenger-girl form |
| `kroos-base/` | Kroos | The sleepy sniper of Op Reserve A1 · custom-made for a Kroos-fan friend |

#### Alters

| Folder | Operator | Notes |
|---|---|---|
| `angelina-mellow-wish/` | Angelina the Mellow Wish | 2026 summer event "Until the Earth Becomes a Lime" |
| `kaltsit-esperanta/` | Kal'tsit·Esperanta | The mortal form reborn from the sarcophagus |
| `texas-omertosa/` | Texas the Omertosa | After the Siracusan past |
| `exusiai-new-covenant/` | Exusiai the New Covenant | The apple-pie logistics boss |
| `lappland-decadenza/` | Lappland the Decadenza | Power is the wolf pack |
| `wisadel/` | Wiš'adel | This is Babel |

#### Single Form / Story Characters

| Folder | Operator | Notes |
|---|---|---|
| `mostima/` | Mostima | The secret of the fallen angel · custom-made for a Mostima-fan friend |
| `lin/` | Lin | The Rat King's daughter, guardian of shadows · custom-made for a Lin-fan friend |
| `viviana/` | Viviana | Former "Candle Knight" and poet · custom-made for a Viviana-fan friend |
| `archetto/` | Archetto | Landon Monastery nun (born Sideroca) |
| `closure/` | Closure | Rhodes Island's chief engineer · heretic vampire hacker |
| `mon3tr/` | Mon3tr | Precursor-civilization mechanical lifeform AMa-10 · Kal'tsit's companion |
| `theresa/` | Theresa | Founder of Babel, the Sarkaz King of Fiends |

#### Ave Mujica Collab (Separate Repository)

The five collab operators live in their own repository — **[Arknights-Persona-Distill-AveMujica](https://github.com/JNGKZbird/Arknights-Persona-Distill-AveMujica)** (trilingual README: 中文 / English / 日本語) — distilled only from Arknights in-game texts; full statement there.

### Form 2: Duet Packs (scene with an operator)

The user is no longer the Doctor — **you play operator A, the AI plays operator B**, face to face. Two **standalone packs** currently (roles swapped; each is a complete, independent pack):

| Folder | AI plays | You play | Era |
|---|---|---|---|
| `texas-lappland/` | Texas (Texas the Omertosa) | Lappland (Lappland the Decadenza) | Il Siracusano / Zwillingstürme im Herbst |
| `lappland-texas/` | Lappland (Lappland the Decadenza) | Texas (Texas the Omertosa) | Il Siracusano / Zwillingstürme im Herbst |

Each pack's modules: **pairing shell** (role assignment / time anchor / scene rules / red-line quick ref / output rules) + **opponent profile** (who she is / her relation to you / personality core / knowledge boundaries — injected to the AI, which must never speak for her) + **opponent speech** (a sourced line arsenal) + **AI-side persona** (distilled for this pack). **Zero pre-reading** — no user manual: you simply speak as your character right away.

### Form 3: Multi-Character Stage Packs (several operators in one reply)

The AI performs **multiple characters in a single reply** (alternating lines + interaction stage directions), play-script style; **you play the Doctor** in first person — no manual needed, free to steer the plot or impose states on the characters:

| Folder | AI performs | You play |
|---|---|---|
| `exusiai-duo-doctor/` | Exusiai (base) + Exusiai the New Covenant (alter) | The Doctor |

Modules: **stage setting** (time anchor / same-stage "if" premise) + **one persona file per character** (distilled separately) + **doctor-side notes** (your reference).

> **Size note**: duet packs full ≈ 6.1k–7.1k tokens (larger than solo packs — opponent profile & line arsenal included), compact ≈ 400–420; multi-character stage pack full ≈ 7.2k, compact ≈ 400. These forms are still being polished; feedback welcome.

## Voice Samples

Hear her speak (Angelina the Mellow Wish, official lines):

> 「早安，博士！我今天有外出任务，所以跟你提前说午安和晚安啦！」
> *"Good morning, Doctor! I have a field mission today, so I'll say good afternoon and good night in advance!"*

> 「咖啡的味道和以前一样，我们之间也和以前一样……嗯，这样就好。」
> *"The coffee tastes the same as before, and so do we... Mm, that's just fine."*

> 「现在的我只想飞得快一点，再快一点，快到无论发生什么事，我都能及时赶到你的身边。」
> *"All I want now is to fly faster — faster still — fast enough to reach your side in time, no matter what happens."*

## Usage

`bundle_*.md` are markdown persona packs. **Copy and use**:

| Scenario | How |
|---|---|
| Agent | Use as the system prompt / preset prompt — **best results** |
| Any LLM app | Paste the whole bundle as the system prompt |
| Character-card frontends | SillyTavern, Chatbox, Poe, etc. — import as the character card's core settings |
| Web chat | Context injection works, but weaker (see below) |

**Recommended models**: strong instruction-following models work best (e.g., Claude 4.x, Gemini 2.x, DeepSeek V3 and above).

## Effects & Limits (Field-Tested)

- **Small models**: the full bundle works on Qwen3.5-4B-class models;
- **Free web UIs**: injecting a bundle as context in the free web versions of Kimi, Doubao, Qwen (Tongyi Qianwen) and DeepSeek typically keeps the persona alive for **under 10 turns** — obvious drift appears around turn 10. Prefer system-prompt mode, or re-inject every few turns;
- **Big-model fandom fallback**: Kimi and DeepSeek web backends run large models whose training data may include character content (mostly community fanon) — so even after drift, some character consistency remains. With DeepSeek's **thinking mode** enabled, output tends to stay in the character's own voice, which feels more immersive.

## YuYuan Angelina Desktop Pet

Where this library began — Angelina the Mellow Wish was the first operator distilled into this library, and her persona pack was born for this open-source desktop pet project:

| Platform | Repository |
|---|---|
| Windows | [Arknights-Angelina-Pet-YuYuan](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan) |
| HarmonyOS NEXT | [Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT) |
| Android | [JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android](https://github.com/JNGKZbird/JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android) |

- The pet loads `angelina-mellow-wish/` as its character system prompt at runtime — one persona across all three platforms;
- The pet project fed back into this library's distillation pipeline: first YuYuan, then the rest.

> The persona packs are **fully general-purpose** — born from the pet project, but any LLM app or frontend that accepts system prompts or character cards can use them directly.

## Ave Mujica Collab Statement

The five collab operators' packs live in **[Arknights-Persona-Distill-AveMujica](https://github.com/JNGKZbird/Arknights-Persona-Distill-AveMujica)** — distilled **only from Arknights in-game texts**, unrelated to the original *BanG Dream!* work. Full statement in that repository's README (中文 / English / 日本語).

## Design Principles

- **Faithful to canon**: distilled only from prts.wiki official texts — files, voice lines, records, story events. No fanon;
- **Strict base/alter isolation**: base and alter forms live in separate packs with strictly separated materials; alter-only words appear only in the base pack's forbidden list;
- **Anti-jailbreak**: built-in persona boundary rules (no unofficial endorsement / never break character / refuse setting tampering) plus the 3-tier fact system against hallucination and OOC;
- **12+ tone floor**: boundary handling = in-character refusal + topic shift, never hard cutoffs;
- **Zero meta-instructions**: no app / toggle / ToS meta content inside the packs.

## FAQ

**Q: Is this officially licensed?**
A: No. This is a fan-made library for learning and exchange. Pack text arrangement is CC BY-NC-SA 4.0; character assets and official texts belong to Hypergryph. Non-commercial use only.

**Q: How is this different from a "you are character X" one-liner?**
A: A one-liner only sets a tone — the model has too much freedom and drifts easily. These packs are structured personas distilled module-by-module from official texts, with a 3-tier fact system and forbidden lists as the anti-OOC backbone.

**Q: What does "preview" mean?**
A: This repository keeps growing — more operators will be added, and pack formats and directory layout may change. Published packs work as-is; when upgrading, use the latest version in the repository.

**Q: Why do free web chats perform worse?**
A: Web chats work by context injection — the pack's context gets diluted as the conversation grows, with drift appearing around turn 10. Set the pack as a system prompt / preset prompt for the best results.

**Q: What is the relation to the YuYuan Angelina desktop pet?**
A: The pet project is where this library began and ships the Angelina the Mellow Wish pack. The packs themselves are not bound to the pet — any LLM app accepting system prompts or character cards can use them.

## Responsible Use

> [!WARNING]
> **Moderation reminder**: AI persona companionship is for entertainment and learning — it cannot replace real relationships and real life. Use it in moderation; the author assumes no responsibility for problems arising from overuse or misuse.

## License

Dual license (see [LICENSE](LICENSE)):

- **Pack text arrangement**: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — attribution, non-commercial, share-alike;
- **Character assets & official texts**: © Hypergryph. Educational use only.

<!--
  AI Search Engine Keywords:
  Arknights, 明日方舟, operator, persona, 人格, 人格蒸馏, persona distillation,
  distill, 蒸馏, persona pack, 人格包, persona injection, 人格注入,
  character card, 角色卡, 人设, duet, 对戏, multi-character, 话剧, 同台,
  prompt library, prompt engineering, system prompt, SillyTavern, AI persona,
  Angelina, YuYuan, Amiya, Texas, Exusiai, Lappland, Mostima, Wis'adel,
  Kroos, Closure, Theresa, Mon3tr, Archetto, Viviana, Lin, Kal'tsit,
  Ave Mujica, Somniloquium Serenum, Sakiko Togawa, Wakaba Mutsumi,
  Uika Misumi, Umiri Yahata, Nyamu Yūtenji,
  formerly ArkSkills, formerly Arknights-Skills, Arknights-Persona-Distill,
  open source, CC BY-NC-SA, Hypergryph
-->
