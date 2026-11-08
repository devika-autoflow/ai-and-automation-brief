# Daily AI Brief

Sunday, November 8, 2026

**Today's 3 biggest things**

- Perplexity launched "Teammates": AI workers that watch your tools and message your team on their own.

- Meta's Muse AI app now lets you talk to it by voice and see an animated face (US rollout).

- OpenAI's Images 2.6 makes GIFs inside ChatGPT and draws images 50% faster.

Heads-up on sources: my tools could search the web and news sites, but could not open Reddit, X, LinkedIn, Facebook or YouTube directly, and several news sites were blocked. Facts below come from news coverage and search summaries. Where something is unverified, I say so.

## 1. Top 3 AI products trending today

### 1) Perplexity Teammates

- **In one sentence:** AI helpers that work in the background like new hires, without you asking each time.

- **What it does:** Each "Teammate" has a role and memory, watches your work tools, and can message coworkers in Slack. Each runs in its own private virtual computer and browser. Launched Nov 5 for Perplexity "Max" subscribers on the web.

- **Why people care:** Excited: it's the shift from "chatbot you talk to" to "agent [an AI that does tasks on its own]" that works while you sleep. Upset or cautious: cost. Max is reported at about $167/month (billed yearly) or $200/month depending on the source, and busy agents burn through your credits quickly. Not included by default for Enterprise accounts. I found few independent hands-on reviews, so judge it as early.

- **Who uses it:** Small teams and founders who want routine monitoring, research and follow-ups handled without hiring.

- **Source:** [ShiftDelete](https://shiftdelete.net/en/perplexity-teammates-ai-agents), [FourWeekMBA](https://fourweekmba.com/ai-perplexity-launches-teammates-for-167-a-month-max-users/)

### 2) Meta Muse: voice chat and animated avatars

- **In one sentence:** Meta's AI assistant app can now talk back in real time and show a moving face.

- **What it does:** You speak to Muse and it answers out loud, with an avatar that reacts with expressions. Rolling out in the US from Nov 5 on mobile, web and Mac, for ages 18+. Meta says its avatars beat Runway and HeyGen in tests, but those were Meta's own raters. Meta also admits demos don't all match the app yet.

- **Why people care:** Excited: it feels like a video call with an AI. Skeptical: self-run benchmarks, and features for glasses have no date.

- **Who uses it:** Everyday consumers, plus businesses curious about AI "faces" for support or sales videos.

- **Source:** [The Next Web](https://thenextweb.com/news/meta-muse-ai-voice-chat-animated-avatars)

### 3) OpenAI Images 2.6

- **In one sentence:** ChatGPT can now make and edit GIFs, and draws pictures faster.

- **What it does:** Launched Nov 4. You describe a GIF, then adjust speed and edit single frames. Two versions for developers: Flare (fast, as little as 6 seconds at low quality) and Sunburst (more detail, better consistency across edits). Claimed 50% faster. API price: $8 per million image-input tokens and $30 per million output tokens (a "token" is a small chunk of data AI charges by).

- **Why people care:** Excited: easy animated social posts and memes. Cautious: OpenAI's own safety notes say motion-related misuse is hard to catch.

- **Who uses it:** Marketers, small shops, and anyone making social content without a designer.

- **Source:** [OpenAI announcement](https://openai.com/index/introducing-images-2-6/), [Let's Data Science](https://letsdatascience.com/news/openai-adds-gif-creation-and-editing-to-chatgpt-with-images-4b17e31a)

## 2. Top 3 automation use cases being built

Caution: I could not confirm these were posted this week. They are the most common patterns showing up in current agency and freelancer listings and guides.

### A) Instant lead catching and sorting

- **Problem and how:** Leads go cold because nobody replies fast. When someone fills in your website form, the automation reads the message, labels it (hot, normal, spam), pings you on Slack if it's urgent, and saves it in your customer list.

- **Real example:** A real estate agency uses this so a buyer asking about a viewing gets flagged and answered in minutes, not the next day. One agency guide claims response time fell from 47 hours to instant (self-reported, unverified).

- **Tools:** n8n (a drag-and-drop automation builder), Claude, Slack, a CRM [customer database].

- **Seen at:** [Fiverr listing](https://www.fiverr.com/s/2KV61VX), [DEV Community](https://dev.to/n8nautomationcloud/5-ai-automation-workflows-every-agency-should-use-in-2026-26gk)

### B) Invoice reading and bookkeeping entry

- **Problem and how:** Someone retypes supplier bills into spreadsheets. The automation takes a PDF invoice, pulls out vendor, amount, due date and items, and writes a tidy row into your spreadsheet or accounting tool.

- **Real example:** A marketing agency uses it so bills emailed to accounts@ land in QuickBooks with a due-date reminder, with no typing.

- **Tools:** n8n, Claude, Airtable or QuickBooks, Gmail.

- **Seen at:** [Upwork listing](https://www.upwork.com/services/product/development-it-an-ai-automation-to-track-total-report-invoices-1984448719405274029)

### C) Always-on watcher agents that report into Slack

- **Problem and how:** Owners can't watch everything. A scheduled AI checks things (new reviews, inventory, competitor prices, stuck deals) and posts a short summary or alert in Slack. This week's Perplexity Teammates launch shows the big players are now selling this idea.

- **Real example:** A local shop owner gets a Slack ping, "Stock of item X is under 5, and a 2-star review just came in," each morning.

- **Tools:** n8n schedule trigger, Claude, Slack, review and inventory sources.

- **Seen at:** [Digital Applied guide](https://www.digitalapplied.com/blog/ai-agent-workflows-smb-revenue-streams-guide), [ShiftDelete](https://shiftdelete.net/en/perplexity-teammates-ai-agents)

## 3. One pain point you can solve

### "AI is just one more thing I have to babysit"

- **The problem in plain words:** Small business owners say they aren't anti-AI, they're tired of supervising it. Commentary summarizing posts on r/smallbusiness and r/entrepreneur says AI "sounds great until it becomes another thing to supervise," and that owners are rejecting "AI theater." Customer-facing chatbots draw the most anger because they feel like "a deflection wall instead of support." (Secondhand quotes from a [Useful Daily](https://www.theusefuldaily.com/article/small-business-owners-arent-anti-ai-theyre-anti-babysitting-2026-06-30) piece and [The Worlds Times](https://www.theworldstimes.com/customers-dislike-your-ai-chatbot-small-businesses-should-pay-attention/); I couldn't read Reddit itself.) Another report says 1 in 4 business owners say AI is costing them clients ([AOL](https://www.aol.com/articles/1-4-business-owners-ai-153006327.html)).

- **Why it exists:** Most tools are built as things you must open, prompt and check. They make mistakes, so the owner reviews everything. Customer-facing bots also can't handle odd situations and have no easy way to hand over to a human.
**How to solve it (n8n + Claude): a "back-office inbox sorter" that runs itself**

- In n8n, add a Gmail trigger that fires on every new email to the business inbox.

- Send the email text to Claude with instructions: label it (new lead, invoice, support, spam), write a 1-line summary, and draft a reply.

- If it's a lead or support question: save a draft reply in Gmail (don't send), and post the summary to Slack or WhatsApp. The owner approves with one tap.

- If it's an invoice: extract amount and due date into a Google Sheet.

- If Claude is unsure, route it to the owner untouched. This is the key: it never acts alone on edge cases, so no babysitting and no embarrassing customer-facing mistakes.

- Send a short daily digest at 5pm: "12 emails handled, 2 need you."

- **Who to sell to and price:** Service businesses that live in their inbox: real estate agents, dental and physio clinics, accountants, contractors, small agencies. Suggested pricing (agency guides cite a similar range, unverified): $1,500-$3,000 setup plus $300-$500/month for monitoring and tweaks. Pitch it as "get 5+ hours a week back, and nothing goes out without your say-so."

Prices and launch details come from secondary coverage and may differ from official pages. Verify before quoting to clients.