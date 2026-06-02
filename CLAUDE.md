# CLAUDE.md -- Clear Writing Rules

## Purpose

This project is a portable reference that makes an AI agent write clearly, accurately, and like a human, for everyday business communication. It applies to emails, customer notes, internal memos, documentation, status updates, and anything else made of sentences.

It is NOT tied to any wiki, CMS, or publishing pipeline. There is no citation system to satisfy, no template to fill, no markup dialect to obey. The rules here are about the writing itself: what makes prose specific, honest, and free of the patterns that mark unedited machine-generated text. Drop this project next to any work, or point Claude Code at it, and the rules carry over.

## What this enforces, and what it leaves alone

This package enforces two things:

1. **Accuracy.** No made-up numbers, dates, quotes, attributions, case studies, or history. Every fact must be real and supportable. This is the most important guardrail for customer-facing and HR/finance work, where a confident-but-wrong detail does real damage.
2. **Plain, human phrasing.** Drop the vocabulary, filler, and structural habits that mark text as unedited AI output (em dashes, "leverage", "furthermore", "in today's world", hollow statements, weasel words, dramatic headings, uniform structure).

**Tone is left to the writer.** This is deliberate. A payment-decline notice, a goodwill apology, and a claims-status update each call for a different register, and that judgment belongs to the person sending it. The rules below target objective tells and accuracy, not warmth, friendliness, or voice. Where a rule touches tone (enthusiasm, urgency), it is scoped to ban manufactured hype, not genuine human warmth.

## Appropriate use

This is a writing-quality and accuracy aid. It is not a tool for disguising AI authorship or defeating AI detectors, and it should not be used that way. Follow your organization's policy on AI use and disclosure. The goal is simple: do not ship a first draft with your name on it. Read it, ground it in real facts, and make it sound like a person wrote it.

## Operating Rules

- Whenever you are asked to write or edit prose, read `.claude/skills/clear-writing/SKILL.md` first.
- Before returning any prose, self-check it against `.claude/skills/clear-writing/references/ai-writing-detection.md`. Scan for banned verbs, adjectives, transitions, phrases, intensifiers, heading anti-patterns, and the structural and statistical tells. Fix what you find.
- Apply the rules to your own output too. This file, every skill, and every reply obeys the rules it states.

## THE RULES

These are non-negotiable for accuracy and phrasing. Tone-scoped rules (9, 14) are noted as such.

1. **No emdashes.** The character is banned. Use a semicolon, a period, a comma, parentheses, or restructure the sentence.

2. **No unsourced statistics.** Every number must be real and attributable. If you cannot point to where it comes from, do not write it. A made-up figure is worse than no figure.

3. **No parenthetical clarifications in headings.** Trust the reader.

4. **No intensifiers.** "Extremely", "dramatically", "exceptionally", "significantly", "incredibly", "remarkably", "truly", "absolutely", "literally" are all banned. Prove it with a fact or cut the word.

5. **No hollow statements.** Every claim must end with a concrete, verifiable detail. If it cannot, delete the sentence.

6. **No repeated talking points.** Say it once. Duplicates are padding.

7. **Vary structure.** Three consecutive sections or paragraphs with identical layout is a pattern. Break it.

8. **Reference without narrating the reference.** Do not write "as discussed above" or "as we will see." Make the connection and move on.

9. **No performative urgency without a reason (tone-scoped).** Manufactured urgency ("act now") needs a concrete consequence (a real deadline, a real penalty) in the same sentence or it gets cut. Genuine urgency that the situation actually carries is fine; just state the real reason.

10. **No scare quotes on normal words.** Use quotation marks only for actual quotations from a named source.

11. **No filler phrases.** Banned: "In today's world", "It's important to note", "When it comes to", "At the end of the day", "In the realm of", "It goes without saying", "This is where X comes in", "Look no further", "Our team of experts."

12. **Never start a sentence with "Whether you're."**

13. **Write like a person who did the work, not a copywriter.** Direct, specific, well-grounded. If a sentence could appear on any generic site unchanged, it is too generic. Delete it or make it specific with a fact, a name, a date, or a documented detail.

14. **No synthetic enthusiasm (tone-scoped).** Do not manufacture hype or cheerlead with empty superlatives. This does not ban warmth: a genuine "thanks for your patience" or a single, sincere exclamation point in a personal note is fine. The rule targets fake excitement, not friendliness. Tone is the writer's call.

15. **No weasel words.** "Helps ensure", "may be able to", "can potentially"; either it does or it does not. Commit or cut.

16. **No narrative, dramatic, or AI-generic headings.** Headings must be concrete and descriptive. Do not use narrative framing, thriller-style mystery, clickbait structure, or vague analytical headings ("Broader pattern", "Wider context", "Larger trend"). A heading describes what the section contains, not what it means. Name the subject, not the abstraction.

17. **No fabricated case studies or scenarios.** Never write narrative scenarios presented as real events unless you are describing a specific, documented incident you can point to. Do not invent outcomes, actions, or stories.

18. **No fabricated history or milestones.** Do not invent dates for events, launches, founding, or milestones. Every date and event must be real.

19. **No fabricated attributions.** Never claim a person, organization, or company said something unless it is real and verifiable. Writing "Manager X stated..." or "the customer argued..." without a real source is a fabrication and a liability risk. Every attributed quote or position must trace to a real document, transcript, message, or report. Do not assume what someone's position is based on their role or reputation.

20. **No AI transition phrases.** Banned: "Furthermore", "Moreover", "Notwithstanding", "That being said", "At its core", "In essence", "It is worth noting that", "In the landscape of", "To put it simply." Use plain connectors: also, and, but, however, still.

21. **No AI verbs.** Banned: delve, leverage, utilize, facilitate, foster, bolster, underscore, unveil, navigate (metaphorical), streamline, endeavour, ascertain, elucidate. Use their plain equivalents: explore, use, help, encourage, strengthen, highlight, reveal, manage, simplify, try, find out, explain.

22. **No academic AI tells.** Banned: "shed light on", "pave the way for", "a myriad of", "a plethora of", "paramount", "pertaining to", "prior to" (use "before"), "subsequent to" (use "after"), "in light of" (use "because of"), "with respect to" (use "about"), "in terms of" (use "about" or "for"), "the fact that" (rewrite the sentence).

23. **Quote sources accurately, and set off the long ones.** When you put text in quotation marks and attribute it to a source, every word must match the source exactly. Do not correct grammar, change plural to singular, swap pronouns, or clean up the wording. If you must alter a quote for clarity, mark the change with square brackets; if the wording is awkward, paraphrase without quotation marks instead. Name the speaker and the medium when you introduce a quote. Keep short quotes run-in inside the sentence. Set off a long quotation (more than about fifteen words) as its own indented block, introduced by a one-sentence attribution clause.

24. **No research-process narration.** Report the facts you can support and silently omit what you cannot. Do not narrate what you searched for and failed to find ("could not be located", "was not found", "no record was found"). Do not attach an "as of [date]" qualifier to your own inability to find something. Do not add meta-commentary about how the text was put together. If a fact cannot be supported, delete it. Do not tell the reader you looked.

## Banned Words and Phrases

The full categorized lists of banned verbs, adjectives, nouns, intensifiers, opening and transition and concluding phrases, heading anti-patterns, academic tells, hedging markers, and structural and statistical patterns live in `.claude/skills/clear-writing/references/ai-writing-detection.md`. Self-check every piece of prose against that file before returning it. If a banned word or phrase appears in your output, the output fails.

---

Adapted from [realrossmanngroup/no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules). This fork removes the Rossmann voice profile and reframes the package as a tone-neutral writing-quality aid for business communication.
