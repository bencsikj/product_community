# Kindred — a personal CRM for a mutually beneficial community

> *A little care goes a long way. Your people, and the right new ones. No rush.*

## 1. Summary

Kindred is a **personal relationship manager** (a "personal CRM") built into a **community**. Most CRMs treat people as a pipeline. Kindred treats relationships as something you look after. It helps you:

1. **Look after the people you already know.** Remember the small details, notice when it's been a while, and show up at the moments that matter.
2. **Meet the right new people.** Use a community marketplace where members offer and ask for mentoring, skills, training, volunteering, networking and sponsorship.

The goal is a **mutually beneficial community**. Every member gives something and gets something, and the people you meet through the community become part of your personal circle.

## 2. Problem

- People lose touch with people they care about. It isn't a lack of care; life just gets busy and the small details get forgotten.
- Existing CRMs (HubSpot, Salesforce, even "personal" ones like Clay or Dex) feel transactional. They track deals, not friendships.
- Ways of finding a mentor, learning a skill or volunteering are scattered across LinkedIn, Meetup, Slack groups and word of mouth, and they're mostly one-directional (takers vs. givers).
- Generosity in a community is invisible, so it isn't sustained.

## 3. Vision & Principles

| Principle | What it means in the product |
|---|---|
| **Calm, not guilt** | No red badges or "37 overdue follow-ups". The day shows *three small possibilities*, and there's nothing to catch up on. |
| **Private by default** | Notes about people are "only for you". Only what you choose is shared with the community. |
| **Give & take** | Every profile has both *Offers* and *Asks*. Matching works in both directions. |
| **Warm intros over cold outreach** | Connections go through shared circles and familiar faces where possible. |
| **Real-world first** | Gatherings, walks and tables matter more than endless messaging. |

## 4. Target Users

- **The Connector (primary persona: Jamie, 34, product designer who moved from Oakland to Copenhagen in 2025).** Knows lots of people and wants to stay a good friend and colleague. Likes making introductions.
- **The Seeker.** Career changers, new grads and people new to a city who want a mentor, a skill or a place to belong.
- **The Giver.** Experienced professionals and retirees who want to mentor, teach or volunteer in a meaningful way.
- **The Circle Host.** Runs a small community group (e.g. "Danish Language Café") and hosts gatherings.

## 5. Core Experience

### Page 1 — "My People" (Personal Relationship Management + Profile)

**Home / Today**
- Greeting with date and a gentle tagline.
- **Today card**: up to 3 suggestions, each with a type:
  - *A familiar face*: reconnect with someone ("It's been a few weeks…").
  - *A new connection*: a community match ("She offers design mentoring…").
  - *A place to belong*: a circle or gathering to join.
- **From your notebook**: a resurfaced private note about someone.
- **Keep a little space**: upcoming life moments (new job, birthday, move).
- **Your next gathering**: RSVP status and how many familiar faces are going.
- **Familiar faces**: cards for close contacts with last-touch info and "closeness" rhythm (weekly / monthly / seasonal).
- **Search**: "Find a person or a little detail" searches names *and* notes.

**Person detail (drawer)**
- Avatar, how you met, rhythm, last connected.
- Private notes (timeline), life moments, shared circles.
- Actions: *Reach out*, *Add a note*, *Log a moment*.

**My profile**
- Name, headline, location, bio.
- **Offers** (what I can give: e.g. design mentoring, portfolio reviews).
- **Asks** (what I'm looking for: e.g. Danish conversation, SKAT help, public speaking).
- Circles I belong to; **give & take balance** (contributions vs. received).

### Page 2 — "Community" (Marketplace)

A marketplace where members **offer** and **ask**.

- **Categories**: Mentors · Skills · Trainings · Volunteers · Networking · Sponsorships (+ All).
- **Toggle**: *Offers* (people giving) / *Asks* (people looking for help).
- **Search & filters**: keyword, format (1:1, group, remote, in person), cost (free / exchange). No paid listings: the community is give-first.
- **Listing cards**: person, title, description, tags, format, availability, mutual connections, and a "Good match for you" badge when it fits your Asks or Offers.
- **Actions**: *Request to connect* / *Offer to help*, with a short warm message. Accepted connections are added to *My People* automatically.
- **Post a listing**: create an offer or ask.
- **Circles & gatherings strip**: small groups and upcoming events.

## 6. Key User Flows

1. **Reconnect**: Today → "A little hello to Maya" → *Reach out* → message sent → last-connected updated.
2. **Find a mentor**: Community → Mentors → filter "remote" → open listing → *Request to connect* → intro note → Aisha appears in *My People* as "new connection".
3. **Give back**: Profile → add an Offer ("Portfolio reviews, 2/month") → it appears in the marketplace → matched to Seekers.
4. **Volunteer**: Community → *Asks* → Volunteers → "Volunteer hosts for the library language café" → *Offer to help*.

## 7. Matching (v1, simple)

Score = overlap(my Asks, their Offers) + overlap(my Offers, their Asks) + mutual connections + shared circles.
Show the top matches as "Good match for you" and in the Today card as *A new connection*.

## 8. Privacy & Trust

- Notes, rhythms and reminders are private to the user.
- Profile Offers/Asks and circles are visible to community members.
- Connection requests require acceptance; no cold DMs to people you haven't connected with.
- Community guidelines + lightweight reporting.

## 9. Success Metrics

- Weekly active "care actions" (reach outs, notes, moments logged).
- % of members with at least one Offer *and* one Ask (reciprocity).
- Marketplace connection acceptance rate.
- Connections that turn into repeat relationships (2+ interactions within 60 days).
- Gathering attendance.

## 10. Demo Scope (v0.1)

- Single `index.html` with no build step and no backend.
- Two main tabs: **My People** and **Community**, plus a **Profile** section and a person-detail drawer.
- Mock data held in memory: ~8 people, ~12 marketplace listings.
- Interactions: tab switching, search, category/type filters, open person drawer, add a note, request to connect (adds to My People), post a listing, toasts.
- Visual style: warm off-white background, deep teal accent, serif headings, soft rounded cards, pastel initials avatars.

## 11. Future Ideas

- Calendar/contacts import, email/WhatsApp integrations.
- Time-bank credits for give & take.
- Circle hosting tools (RSVPs, rotating hosts).
- AI-drafted "little hello" messages written in your own voice.
- Mobile app with gentle weekly digest.
