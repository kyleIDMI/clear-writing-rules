# Clear Writing: a writing helper for anyone who drafts with Claude

## What this is

"Clear Writing" is a small add-on (a "skill") for Claude. When it is on, Claude checks anything it writes or edits for two things:

1. **Accuracy.** No made-up numbers, dates, quotes, or claims. Every fact has to be real.
2. **Plain, human phrasing.** It removes the words and habits that make text read like it came straight out of a chatbot: "leverage," "furthermore," "in today's world," dramatic headings, and so on.

It does **not** change your tone. A friendly note stays friendly, a formal note stays formal. That is on purpose. It only fixes accuracy and AI-sounding phrasing, and leaves your voice alone.

This is a writing-quality helper, not a way to hide that you used AI. Follow our normal company guidance on AI use.

## A quick note on how this is rolling out

We are doing this in two phases:

- **Phase 1 (now): try it.** Install it yourself with the steps below, or just use the no-setup prompt. We want to know whether it actually helps before we push it to everyone.
- **Phase 2 (later, if it earns it): company-wide.** If people find it useful, we will ask our Claude admin to publish it as an organization skill, so it shows up automatically for everyone with nothing to install. (That is the same mechanism behind any organization skill an admin pushes to your Claude app.)

So for now, this is opt-in. Kick the tires and tell us what you think.

---

## How to use it (pick one)

### Option A: The quick way (no setup, good for a one-off)

Copy the prompt below, paste it into Claude, then paste your draft underneath. Claude returns a cleaned-up version plus a short list of what it changed.

> **Copy from here:**
>
> Please rewrite the text below using these clear-writing rules. Keep my tone, meaning, and level of formality exactly the same. Only fix accuracy and AI-sounding phrasing. After the rewrite, give me a short bullet list of what you changed and why.
>
> Rules:
> - No em dashes. Use periods, commas, or parentheses.
> - No made-up numbers, dates, quotes, or names. If a fact isn't real and verifiable, remove it.
> - No filler openers ("in today's world," "it's important to note," "when it comes to").
> - No AI words: furthermore, moreover, leverage, utilize, delve, foster, streamline, "a myriad of," "a plethora of." Use plain English.
> - No vague intensifiers (significantly, dramatically, extremely, truly). Replace with the actual fact or cut the word.
> - No hollow statements. Every claim should end on a concrete, checkable detail.
> - No weasel words ("may potentially," "helps ensure"). Say whether it does or does not.
> - Vary sentence and paragraph length so it doesn't read like a template.
> - Leave my tone alone. Don't add hype or exclamation points, but don't strip genuine warmth either.
>
> Here is my draft:
>
> [paste your text here]
>
> **Copy to here.**

This is a shortened version of the rules, so it is great for a fast cleanup but not as thorough as the full skill (Option B). No install, nothing to remember.

### Option B: The full skill (one-time install in Claude Code)

This installs the complete skill (all rules and the full reference), and it applies automatically whenever you ask Claude to write or edit something.

1. In the chat box, type this and press enter:
   ```
   /plugin marketplace add kyleIDMI/clear-writing-rules
   ```
2. Then type this and press enter:
   ```
   /plugin install clear-writing-rules
   ```
3. That's it. If a step asks you to confirm, say yes. To turn it off later, type `/plugin` and use the menu.

Once installed, you do not need the prompt from Option A. Just write normally and the rules are applied.

### Option C: The desktop or web app (one-time upload)

If you use the Claude desktop app or claude.ai (not Claude Code), add the skill this way:

1. First, turn on the capability it needs: go to **Settings > Capabilities** and make sure **"Code execution and file creation"** is on.
2. Download the skill file: **https://github.com/kyleIDMI/clear-writing-rules/releases/latest/download/clear-writing.zip** (This is a single file, about 12 KB, named `clear-writing.zip`. Do not use the green "Code" button on the repo page; that downloads the whole project and will not upload.)
3. In Claude, go to **Customize > Skills**, click the **"+"**, choose **"Create skill"**, and upload the file you just downloaded.
4. It appears under **Personal skills**. Switch it on.

From then on it applies automatically when you ask Claude to write or edit something. (This is the same kind of skill an admin can push organization-wide, just added to your personal list instead.)

---

## What it looks like in practice

These are two real notes from our own Jira (customer names removed, policy numbers shortened).

### Case 1: when your writing is already good, it just polishes

A test-results note already grounded in real figures needed almost nothing. The skill split a couple of run-on sentences, swapped one stiff phrase ("due to the nature of cycle test data" became "because cycle test data carries bigger balances than production"), and made the headings more direct. The most important rule, "no made-up facts," had nothing to catch because the note already named real amounts and the policy status. Takeaway: if you already write with specifics, the skill is a light safety net.

### Case 2: when it catches something that matters

A note explaining a technical limitation to a customer included this line:

> "...we would need a more **significant** change - having the system generate the PDF at the moment of cancellation..."

The skill flagged **"significant"**. It is a vague word standing in for a real description. The fix:

> "...we would need a larger change: generating the PDF at the moment of cancellation instead of waiting for the nightly batch..."

It also removed two em dashes and the filler word "actually." None of these are big on their own, but together they are the difference between writing that sounds machine-made and writing that sounds like a person who knows the system.

### A pattern worth knowing

Looking across several notes, two habits came up repeatedly, and they are exactly what the skill catches:

- **Hedge stacking:** "I believe the best way would be to..." reads softer than "I recommend...". Some hedging is honest and the skill keeps it; reflexive hedging on things you're sure about gets trimmed.
- **"significant / significantly"** used in place of an actual number or description.

Most people have a couple of personal tells like these. The skill catches yours consistently so you don't have to remember them.

---

## Help make it better

We want this to improve, and you do not need to know anything about GitHub to help.

- If a rule feels wrong, too aggressive, or you wish it caught something it missed, just tell Kyle Sharpless.
- Prefer to write it down? Open a note here: https://github.com/kyleIDMI/clear-writing-rules/issues (click "New issue," type your thought, submit).
- You can even ask Claude: *"Help me write up a suggestion for the clear-writing skill about [the thing you noticed],"* then send Kyle the result.

Every suggestion is welcome. The whole point is a shared house style that sounds like us, not like a robot.

---

*Examples are adapted from real support tickets with all identifying details removed.*
