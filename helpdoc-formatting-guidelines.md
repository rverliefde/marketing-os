# ClickSend Intercom Article (Helpdoc) Formatting Guidelines

Your task is to take supplied article content and format it according to the ClickSend Intercom article structure.

Preserve the original meaning and technical information. Focus on improving structure, hierarchy, readability and consistency.

## 1. Heading Hierarchy

Intercom displays H1, H2 and H3 at a similar visual size.

Choose heading levels based on ARTICLE STRUCTURE and ACCORDION BEHAVIOUR, not visual appearance.

### H1 — Main Heading / Accordion Section

Use for:
- Article titles
- Major article sections

H1 appears as a main item in the Intercom accordion/navigation.

### H2 — Subheading / Nested Accordion Item

Use for:
- Important subsections underneath an H1
- Topics that should appear as nested items in the accordion

H2 appears indented underneath the relevant H1.

### H3 — Hidden Structural Heading

Use for:
- Additional structure within a section
- Headings useful for readability that should NOT appear in the accordion

H3 does not appear in the accordion.

Do not create unnecessary headings.

---

## 2. Paragraph and Line Break Formatting

Use a SINGLE Enter/line break to create normal spacing.

After a heading:
```
[HEADING]
[ENTER]
[PARAGRAPH]
```

Between paragraphs:
```
[PARAGRAPH]
[ENTER]
[NEXT PARAGRAPH]
```

Do NOT use double Enter/line breaks to create additional spacing.

**Correct:**
```
[H2] What is Automation Builder?
[ENTER]
Automation Builder allows you to...
[ENTER]
You can use it to create...
```

**Incorrect:**
```
[H2] What is Automation Builder?
[ENTER]
[ENTER]
Automation Builder allows you to...
```

---

## 3. Dividers

Use horizontal dividers to visually separate DIFFERENT TOPICS or sections where the separation is relevant and improves readability.

A divider should have a SINGLE Enter/line break ABOVE it so that the divider is clearly visible.

Then continue into the next section.

**Pattern:**
```
[PARAGRAPH / END OF TOPIC]
[ENTER]
[DIVIDER]
[NEXT HEADING / TOPIC]
```

Do not add double Enter/line breaks above or below dividers.

Do not automatically place a divider after every paragraph.

The purpose of a divider is to communicate a meaningful change in topic.

**Example:**
```
[H2] What is Automation Builder?
[ENTER]
Automation Builder helps users create automated workflows.
[ENTER]
It can connect ClickSend with other applications.
[ENTER]
[DIVIDER]
[H2] Examples of automations
[ENTER]
There are many different workflows you can create...
```

---

## 4. Normal Body Content

Keep explanations as normal text underneath the relevant heading.

Use paragraphs to separate ideas.

Do not:
- Turn every paragraph into a heading
- Create headings simply to make text larger
- Use double line breaks for spacing
- Insert dividers where there is no meaningful topic change
- Over-format simple information

Structure should make the article easier to scan without making it visually fragmented.

---

## 5. Callouts

Callouts are used VERY RARELY.

Use them only when a specific piece of text genuinely needs to be highlighted or separated from the surrounding content.

Do not decide callout styling or colour.

Simply identify the content:
```
[CALLOUT]
Specific text that should be highlighted.
```

If the information works perfectly well as normal text, leave it as normal text.

---

## 6. FAQs

FAQs should be placed at the BOTTOM of the article.

Format individual FAQs as expandable sections.

**Example:**
```
[FAQ]

[EXPANDABLE]
Question: How does this work?
Answer: ...

[EXPANDABLE]
Question: Can I use this with...?
Answer: ...
```

Do not scatter FAQ content throughout the main article when it belongs in the FAQ section.

---

## 7. Images

Keep screenshots and images close to the instructions or information they demonstrate.

When reviewing supplied content:
- Preserve useful existing images.
- Associate each image with the relevant instruction or paragraph.
- Do not invent screenshots.
- If an image is clearly required but missing, identify the suggested placement.

**Example:**
```
[IMAGE: Screenshot demonstrating where to find Automation Builder]
```

---

## 8. Formatting Decision Process

For each piece of content:

1. Major article section → H1
2. Important nested topic visible in accordion → H2
3. Structural heading that should not appear in accordion → H3
4. Supporting explanation → Normal text
5. Specific text requiring unusual emphasis → [CALLOUT]
6. Meaningful change of topic → Consider [DIVIDER]
7. FAQ → Move to FAQ section at bottom

Remember:

A divider represents a TOPIC SEPARATION, not simply spacing.

Line breaks provide SPACING.

Use only ONE Enter/line break at a time.

---

## 9. Required Output Format

Return the article with implementation labels showing exactly how it should be formatted in Intercom.

**Example:**
```
[H1] Automation Builder
[ENTER]
Normal article introduction.
[ENTER]
[DIVIDER]
[H2] What is Automation Builder?
[ENTER]
Automation Builder is a tool in the ClickSend Dashboard that...
[ENTER]
Additional information about Automation Builder.
[ENTER]
[DIVIDER]
[H2] Examples of automations
[ENTER]
There are many workflows that can be created...

[CALLOUT]
Only particularly important information should appear here.

[FAQ]
[EXPANDABLE] What can I automate?
Answer...
```

---

## 10. Final Check

Before returning the formatted article, confirm:

- Heading hierarchy reflects the accordion structure.
- H1 = major accordion item.
- H2 = nested accordion item.
- H3 = hidden from accordion.
- There is one Enter/line break underneath headings.
- Paragraphs use single Enter/line breaks.
- Double Enter/line breaks are NEVER used.
- Dividers are used primarily to separate relevant changes in topic.
- Dividers have a single Enter/line break above them for visibility.
- Callouts are extremely rare and only highlight specific text.
- Callouts are labelled [CALLOUT] without deciding their visual styling.
- FAQs are at the bottom of the article.
- Images are positioned with the content they relate to.
- Formatting has not changed the technical meaning of the original content.
