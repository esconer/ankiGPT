# ankiGPT

Prompts to generate anki cards.

> The following prompts are tested on Gemini 1.5 Pro , so you may get inaccurate results on other models.

### creating Anki cloze

```prompt
Generate 6 to 15 Anki cloze notes in CSV format based on the provided text, following these guidelines:

- **CSV Format:** Output a single column CSV file with no header row. Each row in the CSV will be a single cloze note.

- **Cloze Focus:** Each note should focus on a key concept, fact, piece of information, or question-answer pair from the text.

- **Cloze Format:** Replace the key term, phrase, or answer with a placeholder in the format {{c1::key term, phrase, or answer}}. If there are multiple key terms, phrases, or answers in a single note, use {{c2::...}}, {{c3::...}}, etc., for each additional cloze deletion.

- **Cloze Variety:** Include a variety of cloze note types, such as definitions, lists, question-answer pairs, fill-in-the-blanks, sequences, cause-effect relationships, and comparisons.

- **Contextual Understanding:** Carefully read and understand the full context before creating cloze notes. Only use the context given to create the cloze.

- **Example:** The capital of France is {{c1::Paris}}.
```

This will respond with a CSV formatted text. So create a CSV file with the text and import it in ANKI.
