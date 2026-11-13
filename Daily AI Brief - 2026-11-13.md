# Daily AI Brief

Friday, 13 November 2026

## Today in 30 seconds

- **Google shipped Gemini 4 Hydrogen** (12 Nov): a faster, cheaper AI built to do multi-step tasks, and free users get it too.

- **Claude Fable 5.2 is cheaper per word but people say each job costs more**, which shows how confusing AI pricing has become.

- **Your best opportunity: chasing unpaid invoices.** 59% of US small businesses have bills over 30 days late, and an n8n + Claude reminder bot fixes that.

## 1. Top 3 AI products trending today

### Gemini 4 Hydrogen (Google)

**In one sentence:** Google's newest ChatGPT-style assistant, tuned to be fast and to actually finish tasks for you instead of just chatting.

**What it does:** You can ask it to write code, sort through documents or work through a job with several steps, such as "research these 5 suppliers and put their prices in a table." Google says it finishes faster and makes up fewer facts than earlier versions. Developers pay $1.50 per million words in and $7.50 per million words out (roughly, since AI pricing is counted in "tokens", which are chunks of words). That's far cheaper than top rivals.

**Why people are talking:** It went live yesterday (12 Nov), and free Gemini app users get it automatically when Google decides a question needs it. The frustration: the news is full of different Gemini 4 names (Hydrogen, Carbon, Argon), and even tech blogs disagree on which one is which.

**Who it's for:** Anyone already on Google Workspace, and developers building automations who want good quality at a low price. For n8n builders, a cheap and fast model means lower running costs on every client workflow.

**Source:** [9to5Google](https://9to5google.com/2026/11/12/gemini-4-hydrogen-launch/) · [Unite.AI](https://www.unite.ai/google-launches-gemini-4-hydrogen-for-everyday-agentic-workflows/)

### Claude Fable 5.2 (Anthropic)

**In one sentence:** The newest top-end version of Claude, an AI assistant built for hard, long jobs like writing software, analysing data and working through complex problems.

**What it does:** It released on 9 Nov. Anthropic says it answers up to 30% faster than the previous version and explains things more clearly. The price per word dropped from $10/$50 to $8/$40 per million tokens. It also did surprisingly well at controlling a simulated two-armed robot, beating most AI systems built specifically for robots.

**Why people are excited and upset:** Fans call it "like the industrial revolution for office workers" (MacRumors comments). Critics say the price cut is misleading. One DEV Community writer found the price per word fell 20% but the cost *per finished task* roughly doubled, because the model "thinks" longer. A top r/ClaudeAI thread was titled *"WTF Fable 5.2 Cost per task is Insane."* Others say they can't tell it apart from the cheaper Opus 5.5 on normal work.

**Who it's for:** Software teams and businesses with hard problems worth paying for. For everyday automations (sorting emails, drafting replies), a cheaper model is still the smart choice. That's a useful point to make to clients worried about AI bills.

**Source:** [MacRumors](https://www.macrumors.com/2026/11/09/anthropic-launches-claude-fable-5-2/) · [@claudeai on X](https://x.com/claudeai/status/2119867138987176141) · [DEV critique](https://dev.to/dishant0406/claude-fable-52-faster-cheaper-and-still-hard-to-justify-6fm)

### ARTEMIS (Google, open source)

**In one sentence:** A free tool that lets you tell an Android phone what to do in plain English, then taps through the apps for you.

**What it does:** You type something like "open the shopping app, add milk to the cart and check out." ARTEMIS looks at the screen, decides what to tap, taps it, checks it worked, and keeps going. Each step takes about 3 to 5 seconds. Reported results say it finished 99%+ of tasks on AndroidWorld (a standard test of 100+ multi-step jobs across 20+ real apps), where most similar tools fail.

**Why people are talking:** It's from Google's Pixel testing team, it's free and open source, and it was one of the top trending GitHub projects for 2–8 Nov. The controversy: articles on Medium allege it copies an existing open-source project called Minitap. Google hasn't responded publicly.

**Who it's for:** App companies that need to test their apps (replacing hours of manual tapping), and automation builders. It also opens the door to automating mobile-only apps that have no API (no official way for software to connect to them).

**Source:** [AlphaSignal](https://alphasignal.ai/news/google-s-artemis-hits-99-on-android-tasks-where-most-agents-fail) · [GitHub README](https://raw.githubusercontent.com/google/artemis/HEAD/README.md)

## 2. Top 3 automation use cases being built this week

### AI receptionist: text back missed calls within 60 seconds

**The problem and fix:** Small businesses miss lots of calls. Vendor studies put it anywhere from 14% to 62% of calls going unanswered, and each missed call is often a lost customer. This automation notices a missed call and texts the person back within a minute ("Sorry we missed you! What can we help with?"). An AI then chats with them, collects their details, books a slot, and logs everything for the owner.

**Real example:** A landscaping company using an n8n version of this reportedly captured 92% of after-hours calls that used to go to voicemail. A real estate agency could use the same setup so that a buyer calling about a listing at 9pm gets an instant text, a few qualifying questions and a viewing slot.

**Tools:** n8n, Twilio (phone/SMS), an AI model (Claude or GPT), Google Calendar, Google Sheets or a CRM (customer database).

**Seen at:** [n8n Community](https://community.n8n.io/t/missed-call-auto-reply-chatbot-for-business-owners/321224) · [GrowwStacks guide](https://growwstacks.com/blog/how-to-create-voice-call-ai-agent-with-n8n)

### One blog post becomes a week of social content

**The problem and fix:** Businesses write a blog post or newsletter and then never share it properly, because rewriting it for each platform takes hours. This automation watches for a newly published post. It then writes a LinkedIn post, a newsletter blurb and three short social captions, and saves them as *drafts* for a human to approve. Nothing goes out unchecked.

**Real example:** A real estate agency publishes "5 things to check before buying in [suburb]." By lunchtime, the marketing person has a ready LinkedIn post, an email blurb and Instagram captions waiting for one-click approval.

**Tools:** n8n, an RSS feed or WordPress trigger, Claude or Gemini, Google Docs / Notion for drafts, Buffer or LinkedIn for scheduling.

**Seen at:** [N8N News, November 2026 (Startup Edition)](https://blog.mean.ceo/n8n-news-november-2026/)

### Inbox sorter with a daily summary

**The problem and fix:** Owners drown in email: enquiries, invoices, spam and supplier updates all mixed together. This automation reads each new email and labels it (new lead / customer issue / bill / ignore). It drafts replies to the common ones and sends the owner one short summary each morning: "3 new leads, 1 angry customer, 2 bills due."

**Real example:** A real estate agency routes every "Is this property still available?" email to the right agent with a pre-written reply ready. The principal gets a 7am digest of everything that needs their personal attention.

**Tools:** n8n, Gmail or Outlook, Claude or Gemini 4 Hydrogen (cheap enough to run on every email), Slack or WhatsApp for the digest.

**Seen at:** [Reddit small-business threads (via The Useful Daily)](https://www.theusefuldaily.com/article/reddit-ai-automation-trust-test-small-business-2026-09-12) · [Jotform n8n agent examples](https://www.jotform.com/ai/agents/n8n-ai-agent-workflow-example/)

## 3. One pain point you can solve

### "I did the work. Why am I begging to get paid?"

**The problem:** Small businesses are drowning in late payments, and chasing them is awkward, slow and exhausting.

- **59%** of US small businesses have invoices more than 30 days overdue, up from 47% last year ([QuickBooks 2026 report](https://quickbooks.intuit.com/r/small-business-data/small-business-late-payments-report-2026/)).

- **Nearly 3 in 10** owners put off paying *themselves* because customers paid late, and **18%** spend more time chasing payments than running the business ([Bluevine survey, 1,052 owners](https://www.bluevine.com/blog/small-business-late-payment-gaps)).

- **Two in five** UK SMEs (small and medium businesses) can't pay staff on time because of late payments ([Bibby 2026](https://www.bibbyfinancialservices.com/knowledge-hub/news/2026/two-fifths-of-smes-can-not-pay-staff-on-time-due-to-late-payment)).

On Reddit, the mood about automation itself is just as telling. Owners are *"tired of tools that promise automation and deliver another maintenance job"* ([The Useful Daily](https://www.theusefuldaily.com/article/reddit-ai-automation-trust-test-small-business-2026-09-12)). So they want this done *for* them, not another app to learn.

**Why it happens:** Nobody likes sending awkward money emails, so reminders go out late, inconsistently, or never. Customers learn they can stall. Accounting software can send reminders, but they're generic templates that get ignored, and no one follows up when a customer replies "I'll pay Friday."

**How to solve it with n8n + Claude:**

- **Every morning**, n8n pulls all unpaid invoices from Xero, QuickBooks or a Google Sheet.

- **Sort by how late they are**: 3 days (friendly nudge), 14 days (firm reminder), 30+ days (final notice and a phone call task).

- **Claude writes a personal email** for each one, using the customer's name, the job done and the amount. It's polite, short and includes a payment link.

- **Owner approves in one tap**: drafts arrive in Slack, WhatsApp or email with "Send / Edit / Skip" buttons. Nothing goes out without a human yes.

- **Watch for replies**: if a customer says "I'll pay Friday", Claude reads it, notes the promise, and schedules a check-in for Friday.

- **Weekly report**: "You're owed $14,200. $6,100 was collected this week. These 3 customers need a call."

**Who to sell this to:**

- Trades and home services (plumbers, electricians, builders): high invoice values and lots of late payers.

- Marketing and design agencies and consultants who bill monthly retainers.

- Bookkeepers and accountants, who can resell it to all their clients. One partner gets you 10–30 businesses.

**What to charge:**

- **Setup:** $750–$1,500 one-off (connect accounting, write the email tone, test).

- **Monthly care plan:** $150–$300/month (you keep it running and fix it if anything breaks). This answers the "another maintenance job" complaint directly.

- **The pitch:** "If this collects one late invoice a month, it pays for itself." With 59% of businesses sitting on overdue bills, that's an easy promise.

Compiled 13 Nov 2026 from tech news, X, Reddit discussion coverage, GitHub trends and the n8n community. Some figures come from vendors and blogs, so check them before quoting to clients.