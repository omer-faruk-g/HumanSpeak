# HumanSpeak

HumanSpeak is a text-rewriting skill for [Claude Code](https://code.claude.com). It is prompt-only: one `SKILL.md`, with no scripts and no hooks. It strips telltale AI vocabulary, robotic transitions and formulaic structure from English and Turkish text and rewrites it to read like a person wrote it.

## Rules

| Section | Rule | What the model does |
|---|---|---|
| 1 | Banned register | It removes generic Turkish openers ("Günümüzde...", "Şüphesiz ki..."), template connectors ("Ayrıca,", "Bunun yanı sıra,"), artificial emphasis ("Kritik bir rol oynamaktadır") and formula closings ("Sonuç olarak,"), and English buzzwords (*delve, tapestry, pivotal, seamlessly...*) and transitions (*Furthermore, Moreover, In conclusion...*). |
| 2.1 | No introductory fluff | The first sentence goes straight to the point, with no dictionary-style definition or generic setup. |
| 2.2 | Varied rhythm | It mixes very short sentences with longer ones instead of uniform 15-20 word sentences. |
| 2.3 | No formula conclusion | It drops closing paragraphs that only restate the text and ends on the last real point. |
| 2.4 | No symmetrical bullets | List items vary in length and form instead of all starting the same way. |
| 2.5 | Concrete over hype | Abstract praise becomes facts, numbers or direct statements. |
| 3 | Pipeline | Scan and scrub, restructure cadence, use direct phrasing, then a final check against common AI-writing patterns. |
| Output | Text only | It returns only the rewritten text, with no list of changes or commentary unless asked. |

## Install

```bash
git clone https://github.com/omer-faruk-g/HumanSpeak ~/.claude/skills/human-speak
```

Then restart Claude Code. The skill loads when you say humanize, insan gibi yaz or HumanSpeak, ask to de-AI a text, or type `/human-speak`.

## Limits

- The final audit is the model's own judgement. It does not run an AI detector, so nothing guarantees the text passes one.
- It changes wording and structure, not facts. If the source text is wrong, the rewrite is still wrong.
- The banned lists are fixed. Some words on them ("Ayrıca", "landscape") are normal in many texts, so the rewrite can drop them where they were fine.
- No measured improvement yet.

## Background

- **Patterns of AI writing:** Wikipedia, [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) (WikiProject AI Cleanup).

## Türkçe özet

HumanSpeak, Claude Code için tek dosyalık bir skill:

- "Günümüzde", "Şüphesiz ki", "Ayrıca", "Sonuç olarak" gibi kalıpları ve İngilizcedeki *delve, pivotal, Furthermore* türü sözcükleri metinden çıkarır.
- İlk cümlede doğrudan konuya girer, cümle uzunluklarını değiştirir, tekrar eden özet paragraflarını siler.
- Abartılı sıfatların yerine somut bilgi ve sayı koyar.
- Yalnızca yeniden yazılmış metni verir; neyi değiştirdiğini anlatmaz.

Yapay zekâ dedektöründen geçeceğini garanti etmez; model metni kendi gözüyle denetler.

Kurmak için yukarıdaki `git clone` komutunu çalıştırın ve Claude Code'u yeniden başlatın.

## License

GPL-3.0-or-later. See [LICENSE](LICENSE).
