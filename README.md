# Ziddi Rebels — AI Research Assistant

**Ever wished a children's book had a chapter about a woman you admire? This tool helps you write it.**

## What is Ziddi Rebels?

*Ziddi Rebels* is a children's book in the spirit of the *Rebel Girls* series: real Indian women who defied expectations, one woman per chapter. Each chapter is a two-page spread — her portrait on the left, and her story plus a few "Did You Know?" surprises on the right. Every story centers on a moment of defiance: the choice she made when the world told her no.

**Why "ziddi"?** *Ziddi* (Hindi: ज़िद्दी, say *ZID-dee*) means stubborn — headstrong, strong-willed, immovable. It's the word Indian girls hear, half-scolding and half-proud, when they won't take no for an answer. This book reclaims it: every woman in these pages was ziddi *for all the right reasons* — stubborn about fairness, about science, about art, about other people. That idea is stitched into every story.

## What does this tool do?

Books like this always leave someone out. The scientist your grandmother used to tell you about. The freedom fighter from your hometown nobody outside it has heard of. The singer, the pilot, the judge — the role model you kept waiting to see on a child's bookshelf and never did.

If you've ever thought *"there should be a chapter about her,"* this tool is for you. It's a set of instructions you give to an AI assistant so it becomes a careful research partner, helping you write her spread yourself — researched, fact-checked, and true. Once it's set up, you name the woman, and the assistant will:

- Ask you a few kickoff questions (who you're writing for, how you like to work)
- Pull together a **research brief** — sourced facts, story angle options, and "Did You Know?" candidates
- **Fact-check** your draft, claim by claim, with sources
- Check the **reading level** against the age group you chose
- Flag style issues (without rewriting your words)
- Help you create **illustration prompts** and **page layout instructions**

One thing it will *never* do: write the story for you, unless you explicitly ask. You're the author. The assistant is the research desk.

## How do I set it up?

Pick the section below that matches the AI you use. All three versions follow the same workflow — choose whichever is easiest for you.

---

### 🖥️ If you use the Claude desktop app

The desktop app can install this as a **skill** — a set of instructions Claude remembers and uses automatically whenever you mention the book or a woman you're profiling.

1. Download [`install/ziddi-rebels.skill`](install/ziddi-rebels.skill) from this repository. (On GitHub, open the file and click the download button.)
2. Open the Claude desktop app.
3. Add the downloaded `ziddi-rebels.skill` file as a skill — you can usually do this by opening the file, or from Claude's skills/capabilities settings.
4. Start a new conversation and say something like: *"I want to write about Janaki Ammal for Ziddi Rebels."*

Claude will recognize the project and start the kickoff questions.

> **A note on plans:** Skill installation may depend on which Claude plan you're on, and this can change over time — please check Claude's current plan details at [claude.ai](https://claude.ai) to confirm what's included in yours.

---

### 🌐 If you use Claude on the web or mobile app (claude.ai)

You can set this up using a **Project** — a workspace on claude.ai where you can save standing instructions that apply to every conversation inside it.

1. On [claude.ai](https://claude.ai), create a new Project (call it "Ziddi Rebels").
2. Open the Project's **custom instructions** (sometimes labeled "Set project instructions").
3. Copy the entire contents of [`install/claude-project-prompt.md`](install/claude-project-prompt.md) and paste it there.
4. Save, then start a new chat inside the Project and name the woman you'd like to write about.

Every conversation in that Project will now follow the Ziddi Rebels workflow.

> Projects may not be available on every Claude plan — check Claude's current plan details at [claude.ai](https://claude.ai) if you don't see the option.

---

### 🤖 If you use any other AI (ChatGPT, Gemini, Mistral, and more)

No special features needed — just a copy and paste.

1. Open [`install/universal-system-prompt.md`](install/universal-system-prompt.md).
2. Copy everything below the "How to use this" note.
3. Paste it as the **first message** of a new conversation (or into a custom-instructions box, if your AI has one — for example, ChatGPT's "Custom GPTs" or Gemini's "Gems").
4. Then, in your next message, name the woman you'd like to write about.

The assistant will follow the same workflow as the Claude versions.

---

### 🧑‍💻 If you use Claude Code (the developer tool)

This repository is also packaged as a Claude Code plugin. In a terminal:

```
git clone https://github.com/myd/ziddi-rebels
claude plugin marketplace add ./ziddi-rebels/plugin
claude plugin install ziddi-rebels@ziddi-rebels
```

If none of those words mean anything to you, you don't need this section — use one of the three options above.

---

## New here? Start with the guides

- **[Getting Started](guides/getting-started.md)** — a walk-through of what your first session looks like, with an example from start to research brief.
- **[FAQ](guides/faq.md)** — common questions from parents and teachers.

## What's in this repository

| File | What it's for |
|------|---------------|
| `install/ziddi-rebels.skill` | The installable file for Claude desktop users |
| `install/claude-project-prompt.md` | Paste into a claude.ai Project's custom instructions |
| `install/universal-system-prompt.md` | Paste into any AI as an opening message |
| `guides/getting-started.md` | A friendly walk-through of your first session |
| `guides/faq.md` | Questions parents and teachers often ask |
| `evals/` | Quality checklists — how to tell if the assistant is doing its job well |
| `plugin/` | The skill's source files, packaged for Claude Code (technical users) |
| `LICENSE` | Creative Commons Attribution 4.0 — free to use and share, with credit |

## How do I know it's working well?

The [`evals/`](evals/) folder holds plain-language quality checklists — one row per thing that should be true about a good research brief, fact-check, or illustration prompt. Print one out and tick it off by hand, or have a second AI conversation grade the first one's work ([instructions here](evals/README.md)). If a row fails, you know exactly what to ask the assistant to redo.

## A word about the stories

Every profile in *Ziddi Rebels* is fact-checked before it's finished — no claim goes in without a source. The assistant is built to be honest about what it can't verify, and to flag problems rather than quietly fix them. The words are always yours.

## License

Everything in this repository is shared under the [Creative Commons Attribution 4.0](LICENSE) license (CC BY 4.0). In plain words: you're free to use it, share it, and adapt it — for your family, your classroom, or your own book project — as long as you credit where it came from.

Happy writing. 🌟
