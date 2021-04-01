---
title: Freelance Content Writer
layout: layout-page-sidenav
---

{% assign jobDetails = site.data.gigs | where: "title", page.title | first %}

{% unless jobDetails.open %}
**The bidding period for this job is over**
{% else %}
<a href="{{ jobDetails.bid_link }}" class="sgds-button is-primary">
  Submit your bid here
</a>
{% endunless %}

### The task

To craft informative and easily digestible articles for the Singapore Government Developer Portal (SGDP) based on GovTech’s community engagement events and products/services. The candidate will be required to understand and make sense of technical content for the articles.

- 1,200 – 1,500 words
- Stylistically similar to NDI piece [link here](https://medium.com/ndi-sg/stack-x-webinar-national-digital-identity-stack-introduction-to-ndi-34b5dbed9565)
- Turnaround for first full draft: 7 working days (5 working days + 2 working days for TMO’s review)

### Timeline

- Two articles for publication on SGDP
  - Publication-ready drafts in Word Doc to be submitted by 30 April 2021
- Option for additional two articles for publication on SGDP
  - Publication-ready drafts in Word Doc to be submitted by 17 May 2021 (negotiable)

### Deliverables

- Article 1: HealthCerts
  - Preparing for Safe Travel: Blockchain’s Opportunities and Challenges
  - From 31 Mar’s panel session with BAS, Steven Koh, Accredify, and Affinidi 
- Article 2: Community Engagement Journey (STACK, STACK-X)

### Skills required

{% for skill in jobDetails.skills %}
- {{ skill }}
{% endfor %}

### Offer

{% include govbuy-offer-table.md 
  offer=jobDetails.offer duration=jobDetails.duration
  posted=jobDetails.posted closing=jobDetails.closing %}

### Evaluation methods

- CV
- Writing portfolio with minimally three articles ranging from 1,000 to 2,000 words; tech content writing is a plus (published content is preferred)