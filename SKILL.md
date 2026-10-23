---
name: human-speak
description: Removes AI signatures, Wikipedia AI templates, robotic transitions, and buzzwords from text. Rewrites content to sound authentic, natural, and human-written. Trigger when user says humanize, insan gibi yaz, HumanSpeak, or asks to de-AI text.
---

# HumanSpeak Protocol — AI Footprint Removal Engine

HumanSpeak transforms AI-generated text into natural, varied, and authentic human writing by stripping out robotic patterns, formulaic structures, and telltale AI vocabulary.

## 1. Banned AI Vocabulary & Phrase Register

Strictly remove and replace the following markers in both English and Turkish:

### Turkish Banned Patterns
- **Jenerik Girişler**: "Günümüzde...", "Son zamanlarda...", "Şüphesiz ki...", "Bildiğiniz gibi...", "Önemli bir yere sahiptir."
- **Şablon Bağlaçlar**: "Ayrıca,", "Bunun yanı sıra,", "Bununla birlikte,", "Öte yandan,", "Netice itibarıyla,"
- **Yapay Vurgular**: "Altını çizmek gerekir ki", "Kritik bir rol oynamaktadır", "Büyük bir titizlikle", "Zengin bir yelpazeli"
- **Formül Kapanışlar**: "Özetle,", "Sonuç olarak,", "Gelecekte bizi nelerin beklediği...", "Tüm bunlar göz önüne alındığında"

### English Banned Patterns
- **AI Buzzwords**: *delve, tapestry, testament, pivotal, beacon, multifaceted, realm, underscore, foster, overarching, seamlessly, paramount, imperative, crucial role, landscape.*
- **Robotic Transitions**: *Furthermore, Moreover, Additionally, Consequently, In summary, Ultimately, It is worth noting that, In conclusion.*

## 2. Structural De-AI-fication Rules

1. **Eliminate Introductory Fluff**: Never start with a dictionary-style definition or generic setup. Jump straight into the subject or core point in Sentence 1.
2. **Break Uniform Rhythms**: AI writes in uniform sentence lengths (15-20 words). Break this by mixing extremely short, punchy sentences with longer, complex thoughts.
3. **Delete Formulaic Conclusions**: Remove summary/conclusion paragraphs that merely rephrase what was already said. End naturally on the last substantive point.
4. **Remove Symmetrical Bullets**: If presenting lists, vary bullet lengths organically. Avoid starting every bullet with the same grammatical structure or bolded title unless explicitly requested.
5. **Concrete Over Hype**: Replace abstract adjectives (*"muazzam bir başarı"*, *"game-changing innovation"*) with concrete facts, numbers, or direct assertions.

## 3. Humanization Pipeline

When processing target text:

1. **Scan & Scrub**: Detect and purge all banned vocabulary and structural markers.
2. **Restructure Cadence**: Vary sentence lengths, use active voice, and connect ideas organically rather than using rigid transitional adverbs.
3. **Inject Authenticity**: Use direct phrasing, practical tone, and natural emphasis.
4. **Final Audit**: Verify the text passes common AI-detector patterns (Wikipedia cleanup standards & forum anti-bot checks).

## Output Requirement
Return ONLY the humanized final text. Do not explain what was changed, do not list deleted words, and do not include meta-commentary unless asked.
