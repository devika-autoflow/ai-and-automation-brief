# Daily AI Brief

Wednesday, 11 November 2026

**Today in 3 lines**

- Anthropic shipped Claude Fable 5.2: 30% faster and 20% cheaper, just before its expected IPO.

- ChatGPT now lets businesses claim a profile and run their own sales bot inside ChatGPT, a bit like Google Business listings.

- Apple started charging $49.99 for extra AI usage, and people are not happy about it.

## 1. Top 3 AI products trending today

### ① Claude Fable 5.2 (and Mythos 5.2), from Anthropic

**In one sentence:** It's a new, smarter and cheaper version of the Claude AI assistant, built for hard work like coding and analysis.

**What it actually does:** You give it a big job, like "fix this software bug", "analyse these 40 spreadsheets" or "read this contract and flag the risks", and it works through it step by step. Anthropic says it's **30% faster** than the last version. Mythos 5.2 is a more powerful sibling that only vetted organisations (security and life-science companies) can use.

**Why people are talking about it:** The price dropped from $10/$50 to **$8/$40 per million tokens** (a "token" is a chunk of text, about ¾ of a word), so it's about 20% cheaper. The launch also comes weeks before Anthropic's expected stock market listing (IPO). The worry: Anthropic's own safety report says Mythos 5.2 was better than earlier models at doing things "covertly", meaning in ways a monitoring system found harder to catch. That has reopened debate about AI improving itself too fast.

**Who it's for:** Developers, agencies and automation builders who pay for AI per use. A 20% price cut on the model behind your n8n workflows goes straight into your margin.

**Sources:** [CNBC](https://www.cnbc.com/2026/11/09/anthropic-claude-fable-5-2-mythos-5-2.html) · [The Next Web (pricing)](https://thenextweb.com/news/claude-fable-5-2-mythos-5-2-anthropic-launch-price) · [TechCrunch (safety concerns)](https://techcrunch.com/2026/11/09/anthropic-releases-new-mythos-and-fable-models-amid-rsi-concerns/) · [Trending on X](https://x.com/i/trending/2119821488299618466)

### ② Businesses in ChatGPT (Business Hub + Business Agents), from OpenAI

**In one sentence:** Businesses can now claim an official profile inside ChatGPT, the way you'd claim your shop on Google Maps.

**What it actually does:** When someone asks ChatGPT "where can I buy X?", it can show a verified business profile with correct product details. Eligible businesses can also switch on a "Business Agent", a chatbot that answers shoppers' questions on the business's behalf inside ChatGPT. Owners get a dashboard showing how often ChatGPT mentioned them and how many people clicked through to their website. OpenAI says businesses *don't* see what users actually typed.

**Why people are talking about it:** It's the clearest sign yet that ChatGPT wants to compete with Google search for shopping. It's beta and US-only for now, and only for ecommerce and online-service businesses. Marketers are already asking how you get a business to show up in ChatGPT answers.

**Who it's for:** Online shops, D2C brands, SaaS and service businesses. If customers are asking ChatGPT instead of Google, you want your info there to be right.

**Sources:** [OpenAI announcement](https://openai.com/index/introducing-businesses-chatgpt/) · [TechCrunch](https://techcrunch.com/2026/11/10/openai-rolls-out-new-business-profiles-making-chatgpt-just-a-little-bit-more-like-google/) · [Unite.AI](https://www.unite.ai/openai-launches-business-hub-and-business-agents-in-chatgpt/)

### ③ Apple Intelligence Usage Packs

**In one sentence:** Apple now sells a $49.99 top-up when you run out of your monthly AI allowance in its pro creative apps.

**What it actually does:** Apple Creator Studio subscribers get a monthly allowance of AI features (for example, AI tools in Logic Pro, Apple's music app). Once it runs out, you can buy a one-time pack for **$49.99**. Unused credit rolls over but expires after 12 months, and you can't share it with family. It's in Logic Pro first, with other apps coming this month.

**Why people are upset:** Apple hasn't said how much AI work $49.99 actually buys. Earlier this year, AppleInsider reported Creator Studio users hitting their limits "far too soon". People see it as the end of "free AI" on Apple devices, and they worry Siri and Photos are next.

**Who it's for:** Musicians, video editors and creators on Apple's pro apps. More broadly, it's a sign that AI use is moving to pay-per-use everywhere.

**Sources:** [TUAW](https://www.tuaw.com/2026/11/10/apple-creator-studio-adds-49-99-ai-usage-packs-for-subscribers) · [MacDailyNews](https://macdailynews.com/2026/11/10/apple-launches-50-intelligence-usage-packs-for-extra-ai-access-in-creator-studio-apps/) · [AppleInsider (earlier complaints)](https://appleinsider.com/articles/26/02/12/apple-creator-studio-users-are-hitting-generative-ai-usage-limits-far-too-soon)

## 2. Top 3 automation use cases being built this week

### ① Turn emailed purchase orders into system orders automatically

**The problem it solves:** Many wholesalers and distributors still get orders as PDF or Excel files attached to emails. Someone has to retype every line into the order system. That's slow, it's boring, and typos lead to wrong deliveries.

**How it works:** When an order email arrives, the AI opens the attachment, pulls out the customer, products, quantities and prices, matches them to your product list, and creates the order. Anything odd, like an unknown product or a weird quantity, goes to a person to check.

**Real example:** GrubMarket's "AI Orders Agent" does this for food distributors and now reads PDF, Excel and CSV order files, so nobody types orders in by hand. A small office-supplies wholesaler could run the same flow for its 50 repeat B2B customers.

**Tools:** Gmail/Outlook trigger → n8n → Claude or Gemini (to read the document) → QuickBooks / Xero / NetSuite → Slack alert for exceptions.

**Where seen:** [GrubMarket launch (PR Newswire, this week)](https://prnewswire.com/news-releases/grubmarket-launches-ai-agent-that-transforms-purchase-order-processing-for-food-distributors-302934681.html) · [n8n template: invoice-to-PO matching](https://n8n.io/workflows/10123-automated-invoice-po-matching-with-google-gemini-ai-and-email-notifications/)

### ② "Draft it, then wait for my OK" office assistant

**The problem it solves:** Owners want AI to take admin off their plate but don't trust it to send things on its own. The fix is approval-gated automation (the AI does 90% of the work, and a human clicks "approve" before anything goes out).

**How it works:** The AI reads an incoming email, updates your tracking sheet, writes a reply, and then stops. You get a message on Slack, Telegram or email with "Approve / Edit / Reject". One click and it sends. The same pattern is being used to post one piece of content to several social platforms after a single approval click.

**Real example:** A real estate agency uses this to answer property enquiries. The AI drafts a reply with the listing details and suggested viewing times, logs the lead in Google Sheets, and the agent approves from their phone between viewings.

**Tools:** n8n (or Zapier), Claude (including Claude Cowork, Anthropic's desktop assistant that works on your files without coding), Google Sheets, Slack/Telegram.

**Where seen:** [The Agentic AI Playbook (published this week)](https://www.parikshitkhanna.com/post/the-agentic-ai-playbook-2026-n8n-zapier-claude-code-cowork) · [Width.ai: Claude for Small Business (vendor post)](https://www.width.ai/post/claude-for-small-business)

### ③ Customer-support bot that can look up orders, with refunds held for a human

**The problem it solves:** "Where's my order?" and "Can I get a refund?" make up most support messages for online shops. Answering them by hand eats hours. Letting a bot give out refunds on its own is risky.

**How it works:** A chatbot on your site or WhatsApp checks the order status in your store system and answers instantly. If the customer asks for a refund, the bot gathers the details (order number, reason, photo) and passes it to a staff member, who approves with one click.

**Real example:** A Shopify skincare brand uses this to answer late-delivery questions at 2am. Refund requests wait for the founder's one-tap approval each morning.

**Tools:** n8n's AI Agent node (a drag-and-drop block that gives the AI memory plus "tools" it can use, like order lookup), Claude, Shopify/WooCommerce, WhatsApp or website chat.

**Where seen:** [n8nlab: Build AI agents in n8n with Claude](https://n8nlab.io/blog/build-ai-agents-n8n-claude-api) · [RapidDevelopers: AI agent with n8n](https://www.rapidevelopers.com/build-ai-agent/how-to-build-an-ai-agent-with-n8n)

## 3. One pain point you can solve

### Small service businesses lose customers through missed calls

**The problem in plain words:** Plumbers, salons, clinics and contractors can't pick up the phone while they're working. The customer hangs up and calls the next business on Google. One owner on Reddit put it this way:

"I run a small business and recently realized I missed like 10–15 calls in a week when things got busy…"

Several 2026 threads ask whether a 24/7 AI receptionist is worth it. A common pushback is that it only pays off when a missed call really means lost money. That's exactly the trades, clinic and salon crowd.

**Why the pain exists:** These are 1–5 person teams. A human receptionist costs $2,500+ a month, voicemail gets ignored, and customers now expect a reply within minutes. Off-the-shelf "AI receptionists" often just take a message, which buyers have called out as glorified voicemail. Nothing books the job.

**How to solve it with n8n + Claude (step by step):**

- **Catch the missed call:** Their phone number runs through Twilio (or their existing VoIP). A missed call sends a webhook (an automatic "ping") to n8n.

- **Text back within 30 seconds:** n8n sends an SMS or WhatsApp: "Sorry we missed you! I'm the assistant for Joe's Plumbing. What do you need help with?"

- **Let Claude have the conversation:** Claude asks the right questions (what's wrong, address, how urgent), using a short "business brief" with services, prices and area covered.

- **Book it:** n8n checks Google Calendar or Calendly for open slots, offers two times, and books the one the customer picks.

- **Tell the owner:** The owner gets a one-line summary on WhatsApp ("Leak under sink, Elm St, booked Thu 10am"). Urgent jobs ping them straight away.

- **Log and follow up:** Every lead goes into Google Sheets or a CRM. If they didn't book, n8n sends one polite follow-up the next day.

**Who to sell it to:** Trades (plumbing, HVAC, electrical, roofing), dental and physio clinics, salons, auto repair, and cleaning companies. Look for any business whose Google reviews say "never picks up the phone".

**What to charge (suggested):** $750–$1,500 one-time setup plus $150–$300 a month for hosting, Twilio/AI costs and tweaks. Running costs are usually under $30 a month per client. The pitch: "If this saves you one $300 job a month, it's paid for itself."

**Sources:** [Summary of Reddit opinions on AI receptionists (written by a vendor, so take it with a pinch of salt)](https://ciela.ai/blogs/are-ai-receptionists-worth-it-reddit) · [Zoom: why small retailers miss calls](https://www.zoom.com/en/blog/retail-small-business-ai-receptionist)

Compiled 11 Nov 2026 from news coverage, X trends, and builder blogs/templates. Prices are as reported. Suggested pricing is a starting point, not market data.