# Lingo Legend Flash Cards

A collection of curated flashcard sets designed for the Lingo Legend language learning app. This repository contains comprehensive vocabulary, grammar, and phrase collections for various languages, formatted according to the official Lingo Legend CSV template.

## Available Flashcard Collections

### Japanese

- **[jlpt_n5_flashcards.csv](jlpt_n5_flashcards.csv)** - Complete JLPT N5 vocabulary and grammar collection
  - 24 topic categories covering all essential N5 content
  - 850+ flashcard entries with comprehensive kanji readings
  - Includes vocabulary, basic grammar patterns, counters, and cultural context

## Official Template

The official Lingo Legend template is included at **[lingo_legend_official_flash_card_template.csv](lingo_legend_official_flash_card_template.csv)**.

### CSV Structure

**Format**: `Topic Name, Topic Description, Topic Type, Native Text, Native Context Line, Translation Text, Translation Context Line, Translation Hint, Pronunciation Override`

### App Constraints

- **Topics**: Unlimited number of topics (unique Topic Name values) allowed
- **Cards per Topic**: Maximum of 100 cards per topic (Lingo Legend app limitation)

**Field Descriptions:**

- **Topic Name** (Required) = The name of the topic category that this card belongs to (e.g., "Basic Conversation").
- **Topic Description** (Optional) = A long description for the topic category (e.g., "In this topic we cover important conversational basics like saying yes and no as well as common courtesies like please and thank you!"). Description & type only need to be specified for the first card in a topic.
- **Topic Type** (Optional) = One of the following allowed options: `0 – Vocab`, `1 – Grammar`, `2 – Phrases`, `3 – Script`, or `4 – Misc`. Description & type only need to be specified for the first card in a topic.
- **Native Text** (Required) = Translation in native tongue.
- **Native Context Line** (Optional) = Short examples or usage notes, when necessary.
- **Translation Text** (Required) = Translation in target language.
- **Translation Context Line** (Optional) = Short examples or usage notes, when necessary.
- **Translation Hint** (Optional) = Phonetic guide or pronunciation aid for the translation text (e.g., hiragana readings for Japanese kanji).
- **Pronunciation Override** (Optional) = Specifies how the app's TTS (text-to-speech) should pronounce the Translation Text field (e.g., romanization or kana for Japanese, phonetic spelling for other languages).

## Language-Specific Guidelines

### Japanese Flash Cards

**Key Rules**:

1. **Kanji Policy**: If Translation Text contains ANY kanji, populate the Translation Hint with the full hiragana reading of the entire Translation Text, preserving punctuation. Pronunciation Override may be left blank if you would like the app to decide on how the kanji should be pronounced.
2. **Topic Metadata**: Only first row of each topic has Topic Description/Type; leave blank for others.
3. **Punctuation**: No terminal 。 for ordinary sentences; keep emphatic marks (！？) when part of expressions.
4. **Context Lines**: Add brief usage notes where helpful (e.g., "Said when toasting", "Polite request"). Use Native Context Line for English-side tags, Translation Context Line for Japanese usage.
5. **Kana-only entries**: Leave Translation Hint and Pronunciation Override blank if no kanji present.

**Examples**:

- `英語が話せますか` → Translation Hint: `えいごがはなせますか`, Pronunciation Override: `えいごがはなせますか`
- `乾杯！` → Translation Hint: `かんぱい！`, Pronunciation Override: `かんぱい！`
- `こんにちは` → Translation Hint: (blank), Pronunciation Override: (blank)

## Contributing

When adding new language collections:

1. Follow the official CSV template structure
2. Create language-specific guidelines (similar to the Japanese section above)
3. Update this README with the new collection details
4. Ensure comprehensive coverage of essential vocabulary and grammar for the target proficiency level
