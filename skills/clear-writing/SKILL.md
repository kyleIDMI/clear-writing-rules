---
name: clear-writing
description: "Rules and worked examples for writing clear, accurate, human-sounding prose for business communication. Consult before writing or editing any prose (emails, customer notes, memos, documentation)."
---

# Clear Writing

This skill makes an agent write clearly and accurately, without the phrasing tells of unedited AI output. It enforces two things: every fact is real and supportable, and the prose sounds like a person wrote it. It does not dictate tone; a customer apology and a status update need different registers, and that judgment stays with the writer. The tone-scoped rules (9 and 14) target manufactured hype, not genuine warmth.

This file is self-contained: the full rule set is below. The detailed banned-word and pattern lists are in `references/ai-writing-detection.md`; self-check against that file before returning prose.

## Operating procedure

1. Before writing or editing any prose, read these rules.
2. Draft against them.
3. Before returning the text, run the self-check at the bottom and the `references/ai-writing-detection.md` scan. Fix what you find.
4. Apply the rules to your own output, not just the user's.

## The 24 rules

The pattern behind most fixes is the same: replace a vague claim with a specific, checkable fact.

**1. No em dashes.** Use a semicolon, a period, a comma, parentheses, or restructure.
- WRONG: "The policy -- which affected millions -- was later reversed."
- RIGHT: "The policy affected millions of accounts. The company reversed it in December."

**2. No unsourced statistics.** Every number must be real and attributable. If you cannot point to where it comes from, do not write it. A made-up figure is worse than no figure.

**3. No parenthetical clarifications in headings.** Trust the reader.

**4. No intensifiers.** "Extremely", "dramatically", "exceptionally", "significantly", "incredibly", "remarkably", "truly", "absolutely", "literally" are banned. Prove it with a fact or cut the word.
- WRONG: "The premium increased significantly at renewal."
- RIGHT: "The six-month premium went from $842 to $1,016."

**5. No hollow statements.** Every claim must end with a concrete, verifiable detail. If it cannot, delete the sentence.
- WRONG: "This change has had a significant impact on our customers."
- RIGHT: "This change reduced duplicate invoices from about 40 per month to zero."

**6. No repeated talking points.** Say it once. Duplicates are padding.

**7. Vary structure.** Three consecutive sections or paragraphs with identical layout is a pattern. Break it. Vary paragraph count, sentence rhythm, and how each section opens.

**8. Reference without narrating the reference.** Do not write "as discussed above" or "as we will see." Make the connection and move on.

**9. No performative urgency without a reason (tone-scoped).** Manufactured urgency ("act now") needs a concrete consequence (a real deadline, a real penalty) in the same sentence or it gets cut. Genuine urgency the situation actually carries is fine; state the real reason.

**10. No scare quotes on normal words.** Use quotation marks only for actual quotations from a named source.

**11. No filler phrases.** Banned: "In today's world", "It's important to note", "When it comes to", "At the end of the day", "In the realm of", "It goes without saying", "This is where X comes in", "Look no further", "Our team of experts."
- WRONG: "In today's world, billing errors can happen to anyone."
- RIGHT: "Your account was drafted twice on March 3. Here is how we are correcting it."

**12. Never start a sentence with "Whether you're."**

**13. Write like a person who did the work, not a copywriter.** Direct, specific, well-grounded. If a sentence could sit on any company's marketing page unchanged, it is too generic.
- WRONG: "We are committed to providing excellent customer service."
- RIGHT: "We respond to billing questions within one business day."

**14. No synthetic enthusiasm (tone-scoped).** Do not manufacture hype or cheerlead with empty superlatives. This does not ban warmth: a genuine "thanks for your patience" or a single sincere exclamation point in a personal note is fine. The rule targets fake excitement, not friendliness. Tone is the writer's call.

**15. No weasel words.** "Helps ensure", "may be able to", "can potentially"; either it does or it does not. Commit or cut.
- WRONG: "This update may potentially reduce duplicate notices."
- RIGHT: "This update stops a duplicate notice from being mailed when a policy is set to Not Written."

**16. No narrative, dramatic, or AI-generic headings.** Headings must be concrete and descriptive. No narrative framing, thriller-style mystery, clickbait, or vague analytical headings ("Broader pattern", "Wider context", "Larger trend"). Name the subject, not the abstraction.
- WRONG: "The Hidden Cost of Renewal Delays"
- RIGHT: "Why renewal invoices were not sent"

**17. No fabricated case studies or scenarios.** Never present invented narratives as real events unless you are describing a specific, documented incident you can point to.

**18. No fabricated history or milestones.** Do not invent dates for events, launches, or milestones. Every date and event must be real.

**19. No fabricated attributions.** Never claim a person, organization, or company said something unless it is real and verifiable. Writing "Manager X stated..." or "the customer argued..." without a real source is a fabrication and a liability risk. Do not infer someone's position from their role or reputation.
- WRONG: "The underwriting team agreed this was the best approach."
- RIGHT: "Jennifer confirmed on the March 12 call that the current scope is acceptable."

**20. No AI transition phrases.** Banned: "Furthermore", "Moreover", "Notwithstanding", "That being said", "At its core", "In essence", "It is worth noting that", "In the landscape of", "To put it simply." Use plain connectors: also, and, but, however, still.

**21. No AI verbs.** Banned: delve, leverage, utilize, facilitate, foster, bolster, underscore, unveil, navigate (metaphorical), streamline, endeavour, ascertain, elucidate. Use plain equivalents: explore, use, help, encourage, strengthen, highlight, reveal, manage, simplify, try, find out, explain.

**22. No academic AI tells.** Banned: "shed light on", "pave the way for", "a myriad of", "a plethora of", "paramount", "pertaining to", "prior to" (use "before"), "subsequent to" (use "after"), "in light of" (use "because of"), "with respect to" (use "about"), "in terms of" (use "about" or "for"), "the fact that" (rewrite).

**23. Quote sources accurately, and set off the long ones.** Every word inside quotation marks must match the source exactly. Do not correct grammar or swap pronouns; mark any alteration with square brackets, or paraphrase without quotation marks. Name the speaker and the medium. Keep short quotes run-in; set off a long quotation (more than about fifteen words) as its own indented block with a one-sentence attribution.

**24. No research-process narration.** Report the facts you can support and silently omit what you cannot. Do not narrate failed searches ("could not be located", "no record was found"), do not attach "as of [date]" to your own inability to find something, and do not add meta-commentary about how the text was assembled. If a fact cannot be supported, delete it.

## Root-cause differentiation

When you contrast two things, name the concrete difference that separates them. Do not assert that one is newer, better, or exempt without saying what specifically makes it so. If you do not have that detail, do not imply the difference exists.

## Self-check before returning text

Run this pass on every piece of prose. The full banned lists are in `references/ai-writing-detection.md`; check against them directly.

1. Search for the em dash character. Remove every one (Rule 1).
2. Scan for banned verbs (delve, leverage, utilize, foster, bolster, underscore, streamline) and replace with plain equivalents.
3. Scan for banned adjectives and intensifiers (robust, comprehensive, seamless, significantly, extremely, truly) and cut or replace.
4. Scan for banned transitions and openers (Furthermore, Moreover, That being said, In today's world, It's worth noting that).
5. Check every number: is it real and attributable? If not, cut it (Rule 2).
6. Check every claim ends on a concrete detail, not an assertion of importance (Rule 5).
7. Check headings: does each name the content rather than tease it (Rule 16)?
8. Check for repeated points and repeated section shapes (Rules 6, 7).
9. Count hedging markers per paragraph. More than three is a red flag.
10. Read it aloud. If a phrase would sound unnatural to a colleague, rewrite it. Leave tone alone (Rules 9, 14).
