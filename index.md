---
title: "Reading Between the Ratings: What 800 Visitor Reviews Told Us"
date: 2026-06-15
---

# Reading Between the Ratings: What 800 Visitor Reviews Told Us
### A data storytelling walkthrough of a visitor feedback analysis

---

## The Backstory

During my internship, one of the things I worked on was analyzing visitor
feedback from a large exhibition — ratings, recommendation responses, and
open-ended comments from people who walked through the event.

The goal wasn't just "what's the average rating" (though that matters too). It
was about figuring out *where* the experience was working, *where* it wasn't,
and *what visitors were actually saying* in their own words.

Since the real dataset is confidential, this article walks through the same kind
of analysis using a synthetic dataset built to mirror the structure and patterns
of the original — same questions, same approach, just fictional numbers and
comments.

---

## What We Were Trying to Find Out

Before touching any numbers, the goal was to answer a few specific things:

1. Overall, how satisfied were visitors?
2. Would they recommend the exhibition to others?
3. Did satisfaction differ depending on which zone people visited?
4. Did age groups experience the event differently?
5. What were people actually *saying* — and how positive or negative was it?
6. Where did visitors come from, in terms of how they heard about the event?

---

## 1. The Big Picture: Are People Happy?

The first thing I looked at was the overall satisfaction score and
recommendation rate — the two headline numbers any organizer wants to know.

| Metric                      | Value |
|------------------------------|-------|
| Average satisfaction (1-5)   | 3.9   |
| Visitors who'd recommend it  | 82%   |

An average of around 3.9 out of 5 isn't bad — it leans positive — but it's also
not a "wow" score. And the recommendation rate backs that up: 82% is solid, but
that remaining 18% is a meaningful chunk of people who walked away unconvinced.
That gap between "decent" and "great" is usually where the more interesting
insights live.

---

## 2. Sentiment: What Were People Actually Saying?

Ratings give you a number, but the open-ended comments tell you the *why*. I
classified each comment as positive, neutral, or negative based on its tone.

| Sentiment | Share of Comments |
|-----------|--------------------|
| Positive  | ~70%               |
| Neutral   | ~25%               |
| Negative  | ~5%                |

The positive comments mostly clustered around things like good organization,
friendly staff, and specific zones being well-curated. The neutral ones were
mostly "it was fine, nothing special" — which is its own signal, honestly.
Visitors who feel "meh" aren't going to actively recommend you, even if they
wouldn't actively complain either.

The negative comments — while only about 1 in 20 — were the most useful. Common
themes included confusing signage, overcrowding on weekends, long queues at
certain stalls, and a few zones feeling under-curated or empty compared to
others. None of these are huge structural problems — they're the kind of thing
that's very fixable with the right attention.

---

## 3. Satisfaction by Zone

Next, I broke satisfaction down by the zone visitors had spent the most time in.

| Zone              | Avg. Satisfaction (1-5) | Recommend Rate |
|-------------------|--------------------------|-----------------|
| Modern Art        | 4.04                     | 84.7%           |
| Tech Innovations  | 3.96                     | 85.2%           |
| Heritage Crafts   | 4.00                     | 79.4%           |
| Photography       | 3.90                     | 83.2%           |
| Food & Culture    | 3.79                     | 80.2%           |
| Kids Zone         | 3.79                     | 80.0%           |

A couple of things stood out here. Modern Art and Tech Innovations scored well on
both satisfaction *and* recommendation — a good sign that the experience there
was consistently strong. Heritage Crafts had a high satisfaction score but a
slightly lower recommend rate, which is an interesting mismatch — people liked it
while they were there, but maybe it didn't leave enough of an impression to
actively talk about afterward.

Food & Culture and Kids Zone — interestingly, two of the busiest zones in terms
of footfall — had the *lowest* satisfaction scores. That's a classic "victim of
its own popularity" pattern: high traffic often means longer queues, more
crowding, and a more stressful experience, even if the actual content is good.

---

## 4. Does Age Group Change the Experience?

I also looked at whether different age groups rated their experience
differently.

| Age Group | Avg. Satisfaction (1-5) |
|-----------|--------------------------|
| 18-25     | 4.01                     |
| 26-35     | 3.94                     |
| Under 18  | 3.89                     |
| 50+       | 3.89                     |
| 36-50     | 3.86                     |

The differences here were fairly small — nothing dramatic — but the 18-25 group
came out slightly ahead, while the 36-50 group was the least enthusiastic. It's a
gentle signal rather than a strong one, but it's worth keeping in mind: if future
programming wants to specifically appeal to the 36-50 age group, it might be
worth digging into *why* that group rated things slightly lower — different
expectations, different interests, or something else.

---

## 5. How Visitors Heard About the Event

Finally, I looked at how people discovered the exhibition in the first place —
useful for thinking about where to focus outreach next time.

| Discovery Source   | Share of Visitors |
|---------------------|--------------------|
| Social Media         | 35%               |
| Friends/Family       | 25%               |
| College/Work         | 20%               |
| Newspaper             | 10%               |
| Online Ads             | 9%                |

Social media and word-of-mouth together accounted for 60% of how people found
out — by far the dominant channels. Traditional advertising (newspaper, online
ads) barely moved the needle. If the goal is to grow attendance next time, this
points pretty clearly toward investing more in social content and
referral-driven outreach rather than traditional ad spend.

---

## Bringing It Together

Looking at all of this side by side, a few clear threads emerged:

- **Overall sentiment is good but not great** — there's a real opportunity to
  move from "decent" to "people are raving about this"
- **Crowded ≠ loved** — the busiest zones (Food & Culture, Kids Zone) had the
  lowest satisfaction, likely due to congestion rather than content quality
- **The negative comments, though few, were specific and actionable** — signage,
  queues, and crowd management came up repeatedly
- **Word of mouth and social media are doing the heavy lifting** for awareness,
  and there's room to lean further into that

What I found most valuable about this kind of analysis is that it doesn't just
tell you *what* happened — it tells you *where to look next*. The ratings flag
the zones worth investigating; the comments tell you what to investigate.

---

## Tools Used

Python (Pandas, NumPy) for the analysis, with a synthetic feedback dataset —
including fictional ratings, recommendation responses, and comments — generated
using Faker to recreate realistic patterns without using any real, confidential
data.

---

*Note: All data used in this article, including ratings, comments, and visitor
details, is synthetically generated for demonstration purposes only. No
confidential or proprietary information from any organization has been used or
disclosed.*
