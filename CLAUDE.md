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

## The rules

The full, self-contained rule set (all 24 rules, with worked examples) lives in the skill itself: `skills/clear-writing/SKILL.md` (mirrored at `.claude/skills/clear-writing/SKILL.md`). That file is the single source of truth, so it travels intact when the skill is installed as a plugin or pushed as an organization skill. This `CLAUDE.md` is the repo entrypoint only; do not duplicate the rule list here, or the two copies will drift.

In short, the rules cover: no em dashes; no unsourced numbers, dates, quotes, attributions, or invented history; no intensifiers, filler phrases, weasel words, AI verbs, or AI transitions; no dramatic headings; vary structure; and quote sources exactly. Rules 9 and 14 are tone-scoped (they ban manufactured hype, not genuine warmth).

## Banned Words and Phrases

The full categorized lists of banned verbs, adjectives, nouns, intensifiers, opening and transition and concluding phrases, heading anti-patterns, academic tells, hedging markers, and structural and statistical patterns live in `.claude/skills/clear-writing/references/ai-writing-detection.md`. Self-check every piece of prose against that file before returning it. If a banned word or phrase appears in your output, the output fails.

---

Adapted from [realrossmanngroup/no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules). This fork removes the Rossmann voice profile and reframes the package as a tone-neutral writing-quality aid for business communication.
