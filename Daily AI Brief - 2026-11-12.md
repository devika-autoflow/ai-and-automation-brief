# Daily AI Brief

Thursday, 12 November 2026 · covers news from 9–11 Nov (nothing major dated 12 Nov had been published at the time of writing)

## Today in 3 lines

- Anthropic shipped Claude Fable 5.2: 30% faster and 20% cheaper than the last version.

- OpenAI let businesses claim a profile inside ChatGPT and put their own AI agent there to answer customers. It's free during the beta.

- The pain to sell this week: missed calls and leads nobody follows up. Fix it with n8n + Claude, which needs no babysitting.

## 1. Top 3 AI products trending today

### ① Claude Fable 5.2 (and Mythos 5.2), from Anthropic

**In one line:** A new version of Claude's "heavy-duty brain", the one you use for long, hard jobs like writing software or digging through big documents.

**What it actually does:** You give it a big multi-step task and it works through it with fewer mistakes than before. Anthropic says it writes its answers up to **30% faster** than version 5.1. Developers pay **$8 per million words-ish of input / $40 per million of output** (technically "tokens", which are small chunks of text). That's **20% cheaper** than 5.1. Mythos 5.2 is the same brain with fewer safety locks on hacking and biology topics, and only vetted security and life-science researchers can use it.

**Why people are talking:** It's faster and cheaper at the same time, which rarely happens. Anthropic says Mythos 5.2 found 10.2% more software security holes than Claude Opus 5.5. Some coverage points out the timing, just before Anthropic's expected IPO (when it starts selling shares on the stock market). Anthropic itself still tells most people to start with Opus 5.5 as their "daily driver", and that has confused some people.

**Who'd use it:** Software teams, agencies building automations, and anyone running long AI jobs. Paying 20% less on every run adds up fast if you build client automations on Claude.

**Source:** [SD Times](https://sdtimes.com/ai/anthropic-introduces-claude-fable-5-2-mythos-5-2/) · [9to5Mac](https://9to5mac.com/2026/11/09/anthropic-upgrades-claude-with-new-fable-5-2-model-details-here/)

### ② "Businesses in ChatGPT", from OpenAI

**In one line:** Think of a Google Business Profile, but inside ChatGPT. Your company gets an official page there, and an AI assistant can talk to customers for you.

**What it actually does:** When someone asks ChatGPT about your shop, salon or software, you control what it says about you. You can also plug in your own AI agent (a bot that can take actions, like answering questions or taking requests, not just chat) so customers talk to it directly. It's in beta (an early test version) and free at launch.

**Why people are excited or upset:** Hundreds of millions of people now ask ChatGPT instead of Google, so this could become the new "be on Google Maps" moment for small businesses. The worry is the same one people had about Google: one more platform you now have to manage, and it could start charging later.

**Who'd use it:** Local businesses, e-commerce stores and SaaS companies (online software sold by subscription). There's also a new service to sell: "we'll set up and run your ChatGPT presence."

**Source:** [Free Press Journal](https://freepressjournal.in/tech/openai-launches-businesses-in-chatgpt-letting-companies-claim-profiles-deploy-ai-agents)

### ③ Gemini 4 Carbon, from Google

**In one line:** Google's newest and smartest AI model is finally opening up beyond a small test group.

**What it actually does:** It's an all-round "thinking" model for reasoning, coding and analysis. It ranks **#1 of 52 models** on the Artificial Analysis Intelligence Index (an independent leaderboard), with a score of 59. This week it reached paying developers and Google AI Ultra subscribers at an introductory **$2 / $10 per million tokens**. Reports say that will rise to $4 / $20 later.

**Why people are excited or upset:** Top-ranked and much cheaper than Claude Fable on paper. But builders were annoyed that it was announced on 28 Oct while almost nobody could use it. One write-up called it "more like a watchlist launch than an immediately deployable model." Some people also expect the price to double once the intro period ends.

**Who'd use it:** Developers and agencies comparing which AI to put behind their products. If the intro price holds, it's worth testing for jobs that process a lot of text.

**Source:** [BuildMVPFast](https://www.buildmvpfast.com/blog/gemini-4-carbon-frontier-model-what-builders-get-2026) · [Latenode](https://latenode.com/news/google-gates-gemini-4-carbon-with-token-prices-set-to-double)

## 2. Top 3 automation use cases being built this week

### ① AI receptionist that answers every call, books the job and follows up

**The problem it solves:** Small service businesses miss calls while they're on a job, and the caller simply rings the next company. Here, an AI voice answers, asks the right questions, checks the calendar, books the appointment and logs everything. If a call is missed, it texts the caller back within a minute.

**Real example:** A real estate agency points its listing phone line at the AI. When a buyer calls at 9pm about a house, the AI answers questions about the listing, books a viewing in the agent's Google Calendar and sends the agent a summary with "hot lead" flagged.

**Tools:** Vapi or Retell AI (the voice), n8n (the "plumbing" that passes data between apps), Claude (writes each business's call script, using details pulled from its Google Maps listing), Google Calendar, Airtable or CRM.

**Where it's being built:** [n8n template: AI voice receptionists with Claude + Vapi + Google Maps](https://n8n.io/workflows/12956-generate-ai-voice-receptionists-for-local-businesses-with-claude-vapi-and-google-maps/) · [n8n template: Vapi + Calendar + Airtable](https://n8n.io/workflows/3427-automate-call-scheduling-with-voice-ai-receptionist-using-vapi-google-calendar-and-airtable/)

### ② Invoices that file themselves, with a human checking only the big ones

**The problem it solves:** Someone spends hours every week typing supplier invoices into spreadsheets or accounting software. Here, invoices that arrive by email or land in a Google Drive folder get read by AI. It pulls out supplier, amount, due date and expense category, then records them. Anything over a set amount, or anything that looks odd, goes to a person for approval.

**Real example:** A 12-person construction firm forwards all supplier PDFs to one inbox. Invoices under $500 go straight into the books. Anything above that pings the owner on Slack or Telegram with "Approve / Reject" buttons.

**Tools:** n8n, Gmail or Google Drive, Claude or GPT (to read the PDF), Google Sheets or QuickBooks, plus Slack or Telegram for approvals.

**Where it's being built:** [n8n's new AI invoice template with expense-code mapping](https://www.createwith.com/tool/n8n/updates/n8n-ships-ai-invoice-processing-template-with-gl-code-mapping) · [n8n invoice agent template #10123](https://n8n.io/workflows/10123)

### ③ One piece of content in, a week of posts and videos out

**The problem it solves:** Businesses know they should post every day but have no time. These pipelines take one source, like a blog post, a YouTube video or a popular Reddit thread, and automatically turn it into LinkedIn posts, X threads and short videos with voiceover and subtitles. They also track what's already been used so nothing gets posted twice.

**Real example:** A dental clinic writes one blog post a week ("5 signs you need a root canal"). The automation turns it into 3 LinkedIn posts, 1 Instagram carousel caption and a 45-second subtitled video. Claude costs about **$0.05 per article**.

**Tools:** n8n, Claude or GPT, a text-to-voice tool, a video editor API, plus a Google Sheet or database to remember what's been posted.

**Where it's being built:** [7-stage Reddit-to-YouTube build, shared on r/n8n this week](https://dev.to/fun_fun_19313eced54af3c68/reddit-to-youtube-automation-in-n8n-the-7-stage-blueprint-2ckg) · [One blog post into 4 pieces of content with Claude (DEV)](https://dev.to/joeytbuilds/the-n8n-workflow-that-turns-one-blog-post-into-4-pieces-of-content-2pa6)

## 3. One pain point you can solve

### The problem: "We never even saw that lead"

Service businesses (plumbers, cleaners, clinics, agencies) pay for ads, then lose the enquiries. Calls go unanswered, web forms sit in an inbox, and "I'll follow up next week" never happens. Here's what owners say:

- One owner said they **missed 20+ calls in a single month**. Another hired a receptionist at **$3,200/month** just to stop it (Reddit posts, quoted by [Trend Seeker](https://trend-seeker.app/ideas/idea_239a1d2d03b2)).

- Leads fall through because *"each person assumed someone else had handled it"* ([TextMyMainNumber](https://textmymainnumber.com/blog/missed-calls-texts-revenue-loss)).

- Owners are fine with AI. What they hate is **babysitting** it: tools that make them check, fix and approve everything ([The Useful Daily, summarising r/smallbusiness](https://www.theusefuldaily.com/article/small-business-owners-arent-anti-ai-theyre-anti-babysitting-2026-06-30)).

- Goldman Sachs data: **93%** of small businesses say AI helps, but only **14%** have it built into how they actually run ([via The Useful Daily](https://www.theusefuldaily.com/article/reddit-smallbusiness-ai-babysitting-tax-2026-07-09)).

Note: the Reddit quotes come second-hand through vendor and commentary sites. The pattern shows up in every source, but I couldn't open the original threads myself.

### Why this happens

Leads come in through 4–5 different doors (phone, website form, Facebook, Google, email). No single person owns them, and the owner is busy doing the actual work. Most "AI tools" they've tried added a new dashboard to watch instead of quietly doing the job.

### How to solve it with n8n + Claude (step by step)

- **Collect every lead in one place.** Connect each lead source (web form, Facebook Lead Ads, Gmail, missed-call alerts from Twilio or the phone system) to one n8n workflow. Every lead becomes one row in a Google Sheet or CRM.

- **Reply within 60 seconds.** Claude writes a short, personal text or email using what the person asked for ("Hi Sarah, saw you need a boiler service in Leeds. I can do Thursday 10am or Friday 2pm, which suits?"). n8n sends it.

- **Score it.** Claude labels each lead Hot, Warm or Cold based on urgency, budget and location. Hot leads ping the owner on WhatsApp or Slack immediately.

- **Follow up on autopilot.** If there's no reply, n8n sends polite nudges at day 1, day 3 and day 7, then stops. Any reply stops the sequence and alerts a human.

- **Weekly report, no dashboard.** Every Monday, Claude emails the owner 5 lines: leads in, replied, booked, lost and why. Nothing to log into, so nothing to babysit.

### Who to sell this to, and what to charge

- **Best buyers:** home-service businesses (HVAC, plumbing, roofing, cleaning), dental and aesthetic clinics, real estate agents, and small marketing agencies. They're all already paying for ads and leaking the leads those ads bring in.

- **Setup:** $1,500–$3,000 one-off (about 1–2 days of build once you have a template).

- **Monthly:** $300–$600/month for hosting, monitoring and tweaks. That's roughly 10–20% of the $3,200/month receptionist they'd otherwise hire.

- **Your pitch:** "If this books just one extra job a month, it pays for itself. And you never have to log into anything."

- **Your running cost:** usually under $30/month per client (n8n hosting + Claude usage + SMS).

Sources are mainly tech news roundups and builder posts from 9–11 Nov 2026. Reddit, X, LinkedIn, Facebook and YouTube could not be read directly. Prices and numbers come from the linked articles. Check them before quoting to clients.