# The Architecture of Thought
A comprehensive test document for **Typora themes**

---

## 1. Typography & Prose

Effective analytical writing demands clarity above all else. The sentence is the unit of thought — not the paragraph, not the section. When we lose control of the sentence, we lose the argument itself.

This paragraph tests **bold emphasis** and *italic tone* side by side. Notice how strong text pulls attention, while italics offer a softer editorial voice. A well-calibrated theme handles both without visual noise.

Here is a longer passage to evaluate line length, leading, and reading comfort across multiple lines of continuous prose. The measure — the width of the text column — determines how many words sit on a line, which in turn shapes reading rhythm. Too wide, and the eye loses its place. Too narrow, and the cadence breaks before a thought can breathe.

---

## 2. Heading Hierarchy

### 2.1 Third-Level Context

The `h3` heading should feel subordinate to `h2` but still carry authority. It introduces a subtopic, not a section.

#### 2.1.1 Fourth-Level Detail

At this level, headings are markers, not structural pillars. They label, but don't divide.

---

## 3. Blockquotes

> **Key insight:** The goal of a theme is not to be noticed — it is to disappear. A good typographic system makes the reader forget they are reading a *styled* document and simply lets the ideas come through.

> This is a second blockquote for comparison. Simpler, no bold, just a reflective note to check spacing between consecutive quote blocks.

---

## 4. Code

Inline code: use `const result = analyze(data)` within a sentence naturally.

A full code block below:

```python
def word_count(text: str) -> dict:
    """Return frequency map of words in text."""
    words = text.lower().split()
    freq = {}
    for word in words:
        freq[word] = freq.get(word, 0) + 1
    return dict(sorted(freq.items(), key=lambda x: -x[1]))
```

And a short JSON snippet:

```json
{
  "theme": "MY WILL v3",
  "mode": "analytical",
  "readability_score": 94
}
```

---

## 5. Tables

| Indicator         | Value     | Trend   | Notes                     |
|-------------------|-----------|---------|---------------------------|
| Reading speed     | 280 wpm   | ↑       | Optimal line length       |
| Comprehension     | 91%       | →       | Stable across sessions    |
| Eye strain index  | Low       | ↓       | Dark mode recommended     |
| Theme version     | 3.0       | —       | Current stable release    |

---

## 6. Lists

**Unordered — principles of analytical writing:**

- Claim first, evidence second
- One idea per paragraph
- Avoid nominalizations where a verb will do
- Read aloud before publishing

**Ordered — revision workflow:**

1. Write the argument without formatting
2. Cut every sentence that doesn't advance the claim
3. Apply structure: headings, lists, emphasis
4. Check the theme renders as intended
5. Export and distribute

---

## 7. Links

Visit the [Typora official documentation](https://support.typora.io) for theme installation details. You can also reference the [CommonMark spec](https://commonmark.org) when writing portable Markdown.

---

## 8. Horizontal Rules as Section Dividers

Used above. Below is a final one before the closing note.

---

## 9. Image Placeholder

*(Replace the URL below with a local image to test rendering, shadow, and border-radius.)*

![Sample image placeholder](https://entura.com.au/wp-content/uploads/2018/05/RottnestIsland-680x300.jpg)

---

## 10. Edge Cases

**Nested list:**

- Category A
  - Subcategory A1
  - Subcategory A2
- Category B
  - Subcategory B1

**Mixed emphasis in a sentence:** This result is *probably* the most **significant finding** in the dataset, though it requires `further_validation()` before publication.

**Long inline code in prose:** The function `calculate_weighted_moving_average(series, window=14, weights=None)` accepts optional weight arrays.

---

*End of test document — Theme v3*
