# Language Families

This document serves as the authoritative research inventory for languages included in the Multilingual Benchmark Explorer.

This inventory is broader than the project's active implementation scope. It identifies languages that may support future comparative work involving tokenization, embeddings, retrieval, evaluation, language contact, morphology, writing systems, and cross-lingual transfer.

Only a small, explicitly identified set of languages will be active in implemented benchmarks at any given time. The current implementation begins with English and Finnish.

Inclusion in this inventory does not mean that every language is under active study or will receive equal coverage. Languages will move into active experiments only when they support a defined AI engineering or evaluation question.

---

# Selection principles

Languages are included because they contribute to one or more of the following research areas:

- multilingual AI engineering
- language family relationships
- language contact
- low-resource NLP
- Indigenous language technologies
- national minority languages
- morphologically rich languages
- multilingual evaluation
- cross-lingual transfer
- writing systems

The language inventory will continue to evolve as the repository grows.

---

# Uralic

## Priority comparison languages

- 🇫🇮 Finnish
- 🇪🇪 Estonian
- 🇸🇪 Meänkieli
- 🦌 North Sámi

## Additional comparison languages

- 🇫🇮 Karelian
- 🇪🇪 Võro
- 🇪🇪 Seto
- 🇱🇻 Livonian
- 🇷🇺 Veps
- 🇭🇺 Hungarian
- 🇷🇺 Erzya
- 🇷🇺 Moksha
- 🇷🇺 Mari
- 🇷🇺 Udmurt

---

# Germanic

## Priority comparison languages

- 🇳🇱 Dutch
- 🇩🇪 German
- 🇸🇪 Swedish
- 🇳🇴 Norwegian
- 🇬🇧 English

## Additional comparison languages

- 🇩🇰 Danish
- 🇮🇸 Icelandic
- 🇳🇱 Frisian
- 🇿🇦 Afrikaans
- ייִדיש Yiddish

---

# Slavic

## Priority comparison languages

- 🇷🇺 Russian
- 🇺🇦 Ukrainian

## Additional comparison languages

- 🇵🇱 Polish
- 🇨🇿 Czech
- 🇸🇰 Slovak
- 🇧🇬 Bulgarian
- 🇷🇸 Serbian
- 🇭🇷 Croatian
- 🇸🇮 Slovenian
- 🇧🇾 Belarusian

---

# Baltic

## Priority comparison languages

- 🇱🇻 Latvian
- 🇱🇹 Lithuanian

---

# Turkic

## Priority comparison languages

- 🇹🇷 Turkish
- 🇦🇿 Azerbaijani

## Additional comparison languages

- 🇷🇺 Tatar
- 🇰🇿 Kazakh
- 🇺🇿 Uzbek
- 🇹🇲 Turkmen
- 🇲🇩 Gagauz

---

# Kartvelian

## Priority comparison language

- 🇬🇪 Georgian

---

# Iranian

## Priority comparison language

- 🇮🇷 Persian (Farsi)

## Additional comparison languages

- 🇦🇫 Dari
- 🇹🇯 Tajik

---

# Northeast Caucasian

## Additional comparison languages

- Lezgin
- Chechen

---

# Other comparison candidates

These languages may support future comparative studies when they align with a defined experiment or evaluation question.

- 🇦🇲 Armenian

---

# Historical languages

Historical languages may occasionally serve as narrowly scoped comparative or historical case studies.

Examples include:

- Old Norse
- Gothic
- Old Church Slavonic
- Old Prussian

---

# Language families and language contact

Language family relationships describe languages that share a common historical ancestry.

Language contact describes how languages influence one another through long-term historical interaction.

Both perspectives are important for multilingual AI engineering.

See:

- `language-contact.md`

---

# Repository connections

This document serves as the authoritative research inventory for the repository. Active benchmark languages are identified separately in the main README and applicable evaluation decisions.

Related documentation includes:

- `languages/README.md`
- `comparative-methodology.md`
- `language-contact.md`
- `low-resource-languages.md`

Individual AI engineering language profiles are located in:

```text
docs/languages/
```

Each language profile follows the standard template documented in:

```text
docs/languages/README.md
```