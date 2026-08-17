# Sample test leads

Twelve cases to paste into the form one at a time. They're deliberately spread across the range so you can see whether the scoring holds up — if everything comes back 8/10, your prompt needs tightening.

Expected category is what a reasonable human would say. The model won't match every time; that's the point of testing.

---

**1 — expect: hot**
Name: Daniel Reyes
Email: daniel@northfieldlogistics.com
Company: Northfield Logistics
Budget: $20,000+
Message: We run a 40-person freight brokerage and our dispatchers are copying load details between three systems by hand. Looking for someone to build an automation layer plus a small internal dashboard. We have budget approved for Q4 and want to start within three weeks.

**2 — expect: hot**
Name: Priya Nair
Email: priya@getbloomhr.io
Company: Bloom HR
Budget: $5,000 - $20,000
Message: Our support inbox gets around 300 emails a week and response time is killing us. We want an AI agent that drafts replies and routes anything it can't handle. We already use Zendesk and n8n internally.

**3 — expect: warm**
Name: Tom Whitaker
Email: tom.whitaker@gmail.com
Company: (blank)
Budget: $1,000 - $5,000
Message: I have an idea for an app that connects local tutors with students. Not sure exactly what's involved but I'd like to talk it through and find out what something like this costs.

**4 — expect: warm**
Name: Aisha Karim
Email: a.karim@medisyncclinics.com
Company: MediSync Clinics
Budget: Not sure yet
Message: We need appointment reminders sent automatically over WhatsApp and missed appointments logged somewhere our front desk can see. Two clinics now, maybe five next year.

**5 — expect: warm**
Name: Marco Ferretti
Email: marco@ferrettidesign.it
Company: Ferretti Design
Budget: $1,000 - $5,000
Message: Need someone to fix and finish a Next.js site another developer abandoned. Roughly 60% done. Can share the repo.

**6 — expect: cold**
Name: Kevin Osei
Email: kevin.osei@outlook.com
Company: (blank)
Budget: Under $1,000
Message: Can you build me a full social media platform like Instagram? I want messaging, video, stories, everything. Budget is tight but there's equity available.

**7 — expect: cold**
Name: Lena Hoffmann
Email: lena@student-tu-berlin.de
Company: (blank)
Budget: Under $1,000
Message: Hi, I'm writing my thesis on workflow automation. Would you be available for a 30 minute interview about how you build these systems?

**8 — expect: cold**
Name: Ryan Patel
Email: ryan@quickflipdeals.net
Company: QuickFlip Deals
Budget: Under $1,000
Message: Need a scraper that pulls product listings from a few sites every hour. Cheapest option please, no fancy stuff.

**9 — expect: spam**
Name: Marketing Team
Email: growth@seo-rank-boost-pro.biz
Company: SEO Rank Boost Pro
Budget: Not sure yet
Message: Hello Sir/Madam, we can put your website on FIRST PAGE of Google in 30 days GUARANTEED. Reply for free audit. Limited time offer!!!

**10 — expect: spam**
Name: asdf
Email: test@test.com
Company: test
Budget: Under $1,000
Message: test test test

**11 — ambiguous, watch this one**
Name: Sarah Lindqvist
Email: sarah@northlight.se
Company: Northlight Studios
Budget: Not sure yet
Message: We're a 12-person animation studio drowning in client revision emails. Not sure if this is even something software can fix, but someone suggested AI might help. Happy to hear what's possible.

**12 — ambiguous, watch this one**
Name: David Okonkwo
Email: dokonkwo@fairwaycapital.com
Company: Fairway Capital
Budget: $20,000+
Message: Interested in discussing a potential engagement. Please send your availability.

---

## What to check

- **11** has no stated budget and hedged language but is a genuinely good lead. If the model scores it cold, your prompt is over-weighting the budget field.
- **12** has a large budget and almost no information. If the model scores it 9/10 purely on budget, same problem in reverse.
- **7** is polite, well-written, and worth nothing commercially. Models often over-score it because it reads professionally.
- **6** mentions equity — a classic signal the model should catch.

If several of these land wrong, adjust the system prompt rather than the threshold. The threshold only moves where the line sits; the prompt is what decides the ordering.

## Capturing evidence

Run all twelve, then screenshot the executions list showing twelve successful runs. That view — a dozen green executions in a row — is more convincing to a client than any single screenshot of the canvas.