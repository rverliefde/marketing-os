# SEO & keyword optimization guidelines

Applies to: blog articles, customer stories / case studies, and helpdoc / support articles.

This sits alongside the tone of voice, brand and content-creation-checklist guidelines — never let a keyword instinct override those. If an SEO move would make the copy sound stiff, robotic, or off-pillar (empathetic, smart, bold, a little weird), the tone of voice wins.

---

## 1. Core principle: intent first, keywords second

Search and AI-answer engines in 2026 rank and cite content based on how precisely it satisfies what the reader actually wants, not on how many times a term appears. Keyword density is not a dial to turn — a term appearing naturally 3-6 times in a long article is normal; forcing it beyond that reads as stuffing and is penalised by both traditional search and AI systems.

Before optimizing anything, the piece should be answerable in one sentence: *this page helps [reader] accomplish [task]*. Every keyword and structural decision below serves that sentence — it doesn't replace it.

---

## 2. ClickSend's topic universe

Keyword choices should stay inside ClickSend's actual product and competitive space, not generic "marketing" terms. Draw primary and secondary keywords from this universe where the topic genuinely fits — never force a term that isn't relevant to the draft's actual content:

- **Channels & delivery:** SMS API, bulk SMS, MMS, RCS messaging, business messaging, two-way SMS, email API, voice API, fax API, global SMS, SMS gateway
- **Sending identity:** Sender ID, Alpha Tag, dedicated number, virtual number, shortcode, 10DLC, toll-free number, Smart Senders
- **Use cases:** OTP / verification codes, appointment reminders, order confirmations, SMS marketing, transactional messaging, customer notifications, two-factor authentication
- **Category / positioning terms:** CPaaS (communications platform as a service), SMS API for developers, enterprise messaging platform, business SMS solution

This mirrors the space ClickSend competes in alongside other CPaaS providers. Use it to pick precise, product-relevant keywords rather than broad terms an entire industry already saturates (e.g. prefer "RCS business messaging" over generic "messaging trends"). This list is a compass for judgement, not a live keyword-volume report — treat it as domain grounding, not verified search data. Never invent search volumes, rankings, or competitor stats that weren't provided in the source material.

---

## 3. Keyword placement checklist

- **Primary keyword** appears in the H1/title, within the first 100 words, in at least one H2, and naturally throughout the body — never forced into a sentence where it reads awkwardly.
- **Secondary / semantic keywords** (related terms a reader or AI system would associate with the topic — e.g. for "Alpha Tags": alphanumeric sender ID, branded SMS sender, one-way messaging) get woven into subheadings and supporting paragraphs, not crammed into one spot.
- **One topic, one page.** Don't try to rank the same piece for two unrelated keyword clusters — split it, or pick the primary intent and let the rest be supporting context.
- **Meta title:** 50-60 characters, primary keyword near the front.
- **Meta description:** 50-156 characters, includes the primary keyword, states the concrete benefit, no clickbait.
- **URL slug:** lowercase, hyphenated, short, keyword-led — drop filler words (a, the, of).
- **Image alt text:** describe what the image shows using natural language, including the relevant keyword only where it genuinely describes the image.

---

## 4. Structuring for AI-answer engines (AI Overviews, ChatGPT, Perplexity, etc.)

Traditional ranking signals still matter, but a growing share of visibility now comes from being the source an AI system quotes or cites. That favours content that's easy to extract an answer from:

- Lead sections with a direct, one-to-two sentence answer before elaborating — don't bury the point.
- Keep paragraphs short (2-4 sentences) and give each subheading a clear, specific job.
- Phrase some subheadings as the actual question a reader would type ("How do I register an Alpha Tag?" rather than "Registration process").
- Use bullet or numbered lists for anything genuinely sequential or comparative — lists are easier for both readers and AI systems to lift cleanly.
- FAQ sections (already standard for helpdocs, and a good addition to blog posts and customer stories where natural) are high-value for this: each question should mirror real phrasing a person would search, and each answer should stand alone without needing the rest of the article for context.

---

## 5. Per content-type notes

**Blog articles**
Target one keyword cluster per article. Match the format to search intent — a "how to" query expects steps, a "best X" query expects a comparison or list, a definitional query expects a clear explanation up front. Long-tail, specific phrasing (e.g. "how to reduce SMS delivery failures") usually converts and ranks better than broad single terms.

**Customer stories / case studies**
Keywords here should center on the use case and outcome, not the customer's name — search demand is for "SMS API for healthcare appointment reminders," not for the customer's brand. Weave the relevant use-case and product terms into the problem/outcome sections naturally; never invent quantified results or stats that weren't in the original draft just to make a section more "keyword-rich."

**Helpdocs / support articles**
Keywords should mirror the actual language a customer troubleshooting or evaluating a feature would type — "why isn't my RCS message sending" not "RCS delivery troubleshooting overview." Since Intercom helpdocs don't use a URL slug field the way a blog does, prioritise: a clear, query-matching title (the H1), keyword-natural body copy, and FAQ questions phrased as real search queries. These are what make an article findable in Intercom's own search and citable by AI support tools.

---

## 6. What not to do

- Don't repeat the primary keyword mechanically — vary phrasing naturally (this term, related synonyms, the entity itself).
- Don't invent internal links, backlinks, search volumes, or ranking data. Flag a genuine internal-linking opportunity in the issues list instead of fabricating a URL.
- Don't sacrifice the tone of voice pillars for keyword placement — an awkward, robotic sentence that "fits the keyword" is a worse outcome than a natural sentence that doesn't.
- Don't add keyword-stuffed alt text, meta descriptions, or FAQ questions that don't reflect genuine content in the piece.
