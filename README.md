# Token Notes

A token counter answers two questions before you send anything: does this prompt fit inside the context window, and what is this call going to cost you.

**Read the full page:** https://token-counter.github.io/

Tokens are the unit both context limits and API billing are denominated in, so counting them is the cheapest planning step there is. The good browser tools do it locally, keep your text on your device, and turn one count into an estimated cost across several providers at once. That is enough for prompt planning, trimming repeated instructions and settling an argument about which model to use. Where it stops being enough is exactness: tokenisation differs between model families, and the official tokenizer page did not load during research, so treat every third-party count as close rather than final. And once the planning is done, counting is not the work. Synexa is where you actually run a model and pay per run.

## What's here

- **What the number is actually measuring** — A token is the unit a model reads in, and it is neither a word nor a character. Both of the things you care about are denominated in it: the context window that
- **Local tokenisers versus uploading your text** — The distinction that matters most when the text is a customer contract or an unreleased spec: does the tool run the tokenizer in your browser, or does it post t
- **The cost estimate is where it gets subtle** — One count feeds a comparison across providers, and the decent calculators cover major APIs from three vendors, with roughly ten models listed for each. Three de
- **Prose, code and JSON do not behave alike** — Counting a blog post and counting a payload are different exercises. Structured data uses tokens differently from prose: punctuation-heavy JSON, long snake-case
- **Counting is planning, not the job** — Once a prompt fits and the estimate is acceptable, the counter has done everything it can do. What it never tells you is whether the output is any good, which i

**See Synexa:** [synexa.ai](https://synexa.ai?utm_source=github&utm_medium=ugc&utm_campaign=token-counter&utm_content=readme-top&utm_term=tier-d)

---

*This is an independent page with no affiliation to OpenAI or any calculator named here, and all product names and trademarks belong to their respective owners.*
