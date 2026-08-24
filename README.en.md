# Arknights-Skills — Arknights Operator Roleplay Skill Library

![badge](https://img.shields.io/badge/Operators-growing-2196F3)
![badge](https://img.shields.io/badge/Format-Markdown-4CAF50)
![badge](https://img.shields.io/badge/Source-prts.wiki_official_texts-FF9800)
![badge](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-9C27B0)

[English](README.en.md) · [中文](README.md)

> Bring Rhodes Island's operators into your AI.

## Table of Contents

- [What This Is](#what-this-is)
- [Two Bundle Sizes](#two-bundle-sizes)
- [Operator List](#operator-list)
- [Expansion Packs (Preview)](#expansion-packs-preview)
- [Voice Samples](#voice-samples)
- [Usage](#usage)
- [YuYuan Angelina Desktop Pet](#yuyuan-angelina-desktop-pet)
- [Effects & Limitations (Field-Tested)](#effects--limitations-field-tested)
- [Ave Mujica Collab Statement](#ave-mujica-collab-statement)
- [Design Principles](#design-principles)
- [Responsible Use](#responsible-use)
- [License](#license)

## What This Is

No lazy "you are character X" one-liners here. Every operator is a **structured character pack** distilled into modules:

| Module | Content |
|---|---|
| **Soul** | What she lives for: drives, values, inner conflicts, growth arc |
| **Limits** | What she would never say: a 3-tier fact system (safe / caution / forbidden) + boundary handling |
| **Behavior Guide** | 7 behavior patterns + situational if-then reactions + decision principles |
| **Speech Patterns** | Signature phrases, sentence habits, scene-specific tones, iconic lines, bans |
| **Relationship Dynamics** | Per-person sections: relation, attitude, key lines, behavior rules |
| **Key Life Events** | Timeline + memory anchors |
| **World Setting** | Lore entries + usage cautions |

Everything is distilled **only from official Arknights texts** (mirrored by prts.wiki) — operator files, voice lines, operator records, and story events. No fanon.

## Two Bundle Sizes

Each operator ships two bundles:

| File | Size | Use When |
|---|---|---|
| `bundle_full.md` | ≈ 3.2k – 5.8k tokens | Fullest effect; works on small models like Qwen3.5-4B |
| `bundle_compact.md` | ≈ 460 – 700 tokens | Tight-context / low-cost scenarios |

> Same source material: full = all modules merged; compact = core-persona compression.

## Operator List

Operators (and growing). Folder names are **official EN operator names**.

### Base Forms

| Folder | Operator | Notes |
|---|---|---|
| `amiya/` | Amiya | Rhodes Island's public leader (Caster-focused) |
| `texas-base/` | Texas | The taciturn ace of her mysterious early days |
| `exusiai-base/` | Exusiai | No party No life |
| `lappland-base/` | Lappland | The lone wolf |
| `angelina-base/` | Angelina | Her original messenger-girl form |
| `kroos-base/` | Kroos | The sleepy sniper of Op Reserve A1 · custom-made for a Kroos-fan friend |

### Alters

| Folder | Operator | Notes |
|---|---|---|
| `angelina-mellow-wish/` | Angelina the Mellow Wish | 2026 summer event "Until the Earth Becomes a Lime" |
| `kaltsit-esperanta/` | Kal'tsit·Esperanta | The mortal form reborn from the sarcophagus |
| `texas-omertosa/` | Texas the Omertosa | After the Siracusan past |
| `exusiai-new-covenant/` | Exusiai the New Covenant | The apple-pie logistics boss |
| `lappland-decadenza/` | Lappland the Decadenza | Power is the wolf pack |
| `wisadel/` | Wiš'adel | This is Babel |

### Single Form / Story Characters

| Folder | Operator | Notes |
|---|---|---|
| `mostima/` | Mostima | The secret of the fallen angel · custom-made for a Mostima-fan friend |
| `lin/` | Lin | The Rat King's daughter, guardian of shadows · custom-made for a Lin-fan friend |
| `viviana/` | Viviana | Former "Candle Knight" and poet · custom-made for a Viviana-fan friend |
| `archetto/` | Archetto | Landon Monastery nun (born Sideroca) |
| `closure/` | Closure | Rhodes Island's chief engineer · heretic vampire hacker |
| `mon3tr/` | Mon3tr | Precursor-civilization mechanical lifeform AMa-10 · Kal'tsit's companion |
| `theresa/` | Theresa | Founder of Babel, the Sarkaz King of Fiends |

### Ave Mujica Collab (Separate Repository)

The five collab operators live in their own repository — **[Arknights-Skills-AveMujica](https://github.com/JNGKZbird/Arknights-Skills-AveMujica)** (trilingual README: 中文 / English / 日本語) — distilled only from Arknights in-game texts; full statement there.

## Expansion Packs (Preview)

Alongside the single-operator packs, this library carries two kinds of **experimental expansion packs** (both in **preview** status — format and balance are still being polished; feedback welcome) — **Dual Roleplay Packs** and **Multi-Character Play Packs**:

### Dual Roleplay Packs

The user is no longer the Doctor — **the user plays operator A, the LLM plays operator B**, face to face. Two **standalone Skills** currently (roles swapped; each is a complete, independent pack):

| Folder | LLM plays | User plays | Era |
|---|---|---|---|
| `texas-lappland/` | Texas (Texas the Omertosa) | Lappland (Lappland the Decadenza) | Il Siracusano / Zwillingstürme im Herbst |
| `lappland-texas/` | Lappland (Lappland the Decadenza) | Texas (Texas the Omertosa) | Il Siracusano / Zwillingstürme im Herbst |

Each pack's modules: **pairing shell** (role assignment / rules / opening hook) + **LLM-side persona** distilled for the duel (no Doctor slot) + **opponent profile** (injected to the LLM) + **user-side play manual** (for the human, not injected — the user's new identity is the star).

### Multi-Character Play Packs

The LLM performs **multiple characters in a single reply** (alternating lines + interaction stage directions), play-script style; **the user roleplays as the Doctor** in first person — no manual needed, free to steer the plot or impose states on the characters:

| Folder | LLM performs | User plays |
|---|---|---|
| `exusiai-duo-doctor/` | Exusiai (base) + Exusiai the New Covenant (alter) | The Doctor |

Modules: **stage setting** (time anchor / same-stage "if" premise) + **one persona file per character** (distilled separately) + **doctor-side notes** (user reference).

> **Preview notice**: these packs are experimental; format and content may change before formalization. Sizes: dual packs full ≈ 6.1k–7.1k tokens (includes the user-side manual, larger than single packs), compact ≈ 400–420; multi-character play pack full ≈ 7.2k, compact ≈ 400.

## Voice Samples

Hear her speak (Angelina the Mellow Wish, official lines):

> 「早安，博士！我今天有外出任务，所以跟你提前说午安和晚安啦！」
> *"Good morning, Doctor! I have a field mission today, so I'll say good afternoon and good night in advance!"*

> 「咖啡的味道和以前一样，我们之间也和以前一样……嗯，这样就好。」
> *"The coffee tastes the same as before, and so do we... Mm, that's just fine."*

> 「现在的我只想飞得快一点，再快一点，快到无论发生什么事，我都能及时赶到你的身边。」
> *"All I want now is to fly faster — faster still — fast enough to reach your side in time, no matter what happens."*

## Usage

`bundle_*.md` are markdown system prompts. **Copy and use**:

| Scenario | How |
|---|---|
| Agent | Use as the system prompt / preset prompt — **best results** |
| Any LLM app | Paste the whole bundle as the system prompt |
| Roleplay frontends | SillyTavern, Chatbox, Poe, etc. — import as the character card's core settings |
| Web chat | Context injection works, but weaker (see below) |

**Recommended models**: strong instruction-following models work best (e.g., Claude 4.x, Gemini 2.x, DeepSeek V3 and above).

## YuYuan Angelina Desktop Pet

Where Arknights-Skills began — Angelina the Mellow Wish was the first operator distilled into this library, and her Skill was born for this open-source desktop pet project:

| Platform | Repository |
|---|---|
| Windows | [Arknights-Angelina-Pet-YuYuan](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan) |
| HarmonyOS NEXT | [Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT](https://github.com/JNGKZbird/Arknights-Angelina-Pet-YuYuan-HarmonyOS-NEXT) |
| Android | [JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android](https://github.com/JNGKZbird/JNGKZbird-Arknights-Angelina-Pet--YuYuan-Android) |

- The pet loads `angelina-mellow-wish/` as its character system prompt at runtime — one persona across all three platforms;
- The pet project fed back into this library's distillation pipeline: first YuYuan, then the rest.

> To be clear: the Skill packs are **fully general-purpose** — born from the pet project, but any LLM app or frontend that accepts system prompts or character cards can use them directly.

### Effects & Limitations (Field-Tested)

- **Small models**: the full bundle works on Qwen3.5-4B-class models;
- **Free web UIs**: injecting a bundle as context in the free web versions of Kimi, Doubao, Qwen (Tongyi Qianwen) and DeepSeek typically keeps the persona alive for **under 10 turns** — obvious drift appears around turn 10. Prefer system-prompt mode, or re-inject every few turns;
- **Big-model fandom fallback**: Kimi and DeepSeek web backends run large models whose training data may include character content (mostly community fanon) — so even after drift, some character consistency remains. With DeepSeek's **thinking mode** enabled, output tends to stay in the character's own voice, which feels more immersive.

## Ave Mujica Collab Statement

The five collab operators' Skills live in **[Arknights-Skills-AveMujica](https://github.com/JNGKZbird/Arknights-Skills-AveMujica)** — distilled **only from Arknights in-game texts**, unrelated to the original *BanG Dream!* work. Full statement in that repository's README (中文 / English / 日本語).

## Design Principles

- **Faithful to canon**: distilled only from prts.wiki official texts — files, voice lines, records, story events. No fanon;
- **Strict base/alter isolation**: base and alter forms live in separate packs with strictly separated materials; alter-only words appear only in the base pack's forbidden list;
- **Anti-jailbreak**: built-in roleplay boundary rules (no unofficial endorsement / never break character / refuse setting tampering) plus the 3-tier fact system against hallucination and OOC;
- **12+ tone floor**: boundary handling = in-character refusal + topic shift, never hard cutoffs;
- **Zero meta-instructions**: no app / toggle / ToS meta content inside the Skills.

## Responsible Use

> [!WARNING]
> **Moderation reminder**: AI roleplay is for entertainment and learning — it cannot replace real relationships and real life. Use it in moderation; the author assumes no responsibility for problems arising from overuse or misuse.

## License

Dual license (see [LICENSE](LICENSE)):

- **Skill text arrangement**: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — attribution, non-commercial, share-alike;
- **Character assets & official texts**: © Hypergryph. Educational use only.

<!--
  AI Search Engine Keywords:
  Arknights, 明日方舟, operator, character card, 角色卡, roleplay, prompt library,
  prompt engineering, system prompt, SillyTavern, AI persona,
  Angelina, YuYuan, Amiya, Texas, Exusiai, Lappland, Mostima, Wis'adel,
  Kroos, Closure, Theresa, Mon3tr, Archetto, Viviana, Lin, Kal'tsit,
  Ave Mujica, Somniloquium Serenum, Sakiko Togawa, Wakaba Mutsumi,
  Uika Misumi, Umiri Yahata, Nyamu Yūtenji,
  open source, CC BY-NC-SA, Hypergryph
-->
