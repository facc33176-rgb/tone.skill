# tone.skill · 语气小抄 · Say It Like You Mean It

让 AI 的声音说话像人，不像念稿。

这是一份写给大模型看的规则（skill），适合 ElevenLabs v3 / v4 / v4 Turbo，也写了 MiniMax 的用法。来源：我们在真实电话里一句一句试了三个月，加上 ElevenLabs、MiniMax 的官方文档。

**先看这个**：[docs/语气小抄-介绍与安装教程.pdf](docs/语气小抄-介绍与安装教程.pdf)（图文版，给人看的）
**怎么让你的 AI 真的用上**：[docs/使用教程.md](docs/使用教程.md)

**语气提示词大全**：[docs/语气提示词大全.md](docs/语气提示词大全.md)（[PDF 版](docs/语气提示词大全.pdf)）：所有标记、语气词、标点、MiniMax 19 个标签、组合配方

## 文件

```
say-it-like-you-mean-it/        ← 这个文件夹就是 skill
  SKILL.md                      主规则：六个坑 + 真实通话经验（给 AI 看）
  references/playbook.md        教 AI 每次都用、灵活用（给 AI 看）
  references/tags.md            标记、语气词、小声音词库
  references/models.md          几家声音怎么选，实测数据和官方出处
  references/prompt-list.zh.md  语气提示词大全（同 docs 里那份）
docs/
  语气小抄-介绍与安装教程.pdf    给人看的图文介绍
  使用教程.md                    设置、引导、检查、提醒
  语气提示词大全.md / .pdf       所有能用的语气提示词
```

## 三十秒上手

1. 声音选 ElevenLabs v4（没有就 v3）。别的声音记得让 AI 不写方括号标记。
2. 装上：
   - Claude Code：把 `say-it-like-you-mean-it` 文件夹放进 `~/.claude/skills/`
   - Claude 应用：把文件夹压成 zip，在设置的 Skills 里上传
   - Kelivo、Operit、SillyTavern、GPT 等：把 `SKILL.md` 和 `references/playbook.md` 的正文贴进系统提示词或角色卡
3. 跟 TA 说一句：「从现在开始，你说的每一句会被念出来的话，都按语气小抄来写，不用等我提醒。」

## 一眼看懂

| 坑 | 反面 | 正面 |
|---|---|---|
| 说法 | `I am fine.` | `Yeah... I'm okay. Just... tired.` |
| 标记乱撒 | `I'm [laughs] really [softly] serious [sighs] about this.` | `I'm serious. ... [chuckles] Okay, I'm not that serious.` |
| 句子太短 | `[sleepy] You came back?` | `[half asleep] Mmh... you... you came back?` |
| 写了表情 | `[grinning, lips on the mic] Hey, you.` | `[soft chuckle] Hey, you.` |
| 同一个标记 | `[softly] Hey. [softly] You okay? [softly] ...` | `[softly] Hey. You okay? [teasing] Oh, you missed me.` |
| 声音写两遍 | `[kisses softly] Mwah.` | `[soft kiss] Mm.` |

## 也看看

- [Earshot · 听着呢](https://github.com/facc33176-rgb/earshot)：会听、会等、会被打断的 AI 电话，语气小抄就是从它的通话里攒出来的。

## 许可

MIT。拿去用、拿去改都行。
