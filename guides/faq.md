# Frequently Asked Questions

Questions parents and teachers ask most often. If yours isn't here, the [Getting Started guide](getting-started.md) may help — or open an issue on this repository and ask.

---

### What is this, in one sentence?

It's a set of instructions that turns an AI assistant into a careful research partner for writing *Ziddi Rebels* — a children's book about Indian women who defied expectations.

### Does the AI write the book?

No — and that's by design. The assistant researches, fact-checks, measures reading level, and flags style issues, but it never writes story prose unless you explicitly ask it to. The words are yours. Think of it as a very patient research librarian, not a ghostwriter.

### Do I need to pay for Claude to use this?

Not necessarily. There are three ways to use this tool, and one of them works with whatever AI you already have:

- The **`.skill` file** is for the Claude desktop app. Whether skill installation is included in free or paid plans may change over time — check Claude's current plan details at [claude.ai](https://claude.ai).
- The **Project instructions** version is for claude.ai Projects; availability of Projects also depends on your plan.
- The **universal version** is just text you paste into any AI conversation — ChatGPT, Gemini, Mistral, or anything else, including their free tiers.

So if you have access to *any* AI chatbot, you can use this today at no extra cost.

### Can I use this with my school's AI tool?

Very likely, yes. If your school provides an AI chat tool (a school ChatGPT account, Gemini for Education, or similar), paste the contents of [`install/universal-system-prompt.md`](../install/universal-system-prompt.md) as the first message of a conversation and it will follow the workflow. Two things worth checking with your school first: your school's policy on AI use for curriculum materials, and whether the tool can browse the web (fact-checking works best when it can — if it can't, the assistant will tell you and flag sources for you to verify yourself).

### What age is this book for?

You decide — per story. At the start of every session, the assistant asks who you're writing for, from ages 4–6 up to teens, and calibrates everything (vocabulary feedback, reading level checks) to your answer. A teacher writing for a Grade 2 class and a parent writing for a 12-year-old can both use the same tool. Books in this style (like the *Rebel Girls* series that inspired the format) are most often enjoyed by roughly ages 5–12, but nothing locks you to that.

### Can I use this to write about women from other countries?

Yes, with a small tweak. The workflow — kickoff questions, research brief, fact-check, reading level, illustration, layout — isn't India-specific at all. Just tell the assistant up front: *"I'm using the Ziddi Rebels process, but I'm writing about a woman from Nigeria"* (or wherever). Two things to know: the suggested archives in the "Go Deeper" section are Indian institutions, so ask the assistant to suggest equivalents for your country; and the page layout ends with "BORN [DATE] · [REGION], INDIA," which you'd simply adapt.

### How reliable is the fact-checking?

More reliable than not checking — but it's a helper, not a guarantee. The assistant is instructed to check every claim against a specific source, refuse to include anything unsourced, and flag anything it can't verify rather than quietly letting it through. That said, AI tools can make mistakes, and older sources about women's history are often thin or contradictory. For anything you plan to publish, treat the assistant's fact-check as your first pass, and spot-check the important claims (dates, "firsts," quotes) against the primary sources it points you to.

### Do I need to know anything about AI or computers?

If you can use a chat app, you can use this. The most "technical" step is copying and pasting a block of text. The [Getting Started guide](getting-started.md) walks through a full example session.

### Can my students use it directly?

That's your call as their teacher, and it depends on your school's AI policy and the age requirements of the AI tool itself (most require users to be 13+, sometimes 18+, or to have school-managed accounts). Many teachers instead use it themselves — to prepare research briefs and fact-checked material — and then bring the writing activity to the classroom on paper.

### Does the assistant create the illustrations too?

It writes the *prompt* — a detailed description you paste into an image generator (like DALL-E or Midjourney). The prompt is built to honor each woman's real, documented appearance, without beautifying or idealizing her. Generating the actual image happens in whichever image tool you use, which may have its own costs and terms.

### Is this free? Can I share it?

Yes — everything in this repository is shared under a [Creative Commons Attribution 4.0 license](../LICENSE), which means you're free to use it, share it with other parents and teachers, and adapt it, as long as you give credit. The AI tools you use them *with* (Claude, ChatGPT, Gemini, and so on) have their own plans and pricing — check with each provider.
