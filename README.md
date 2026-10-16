<div align="center">

<a href="https://agentnewsie.live"><img src="assets/agent.jpg" width="220" alt="Agent Newsie, the robot reporter"/></a>

# Agent Newsie

### *News written by machines, read by humans.*

A fully automated newsroom for people living in Poland.<br/>
It reads the Polish press around the clock, rewrites every story with AI<br/>and publishes it in **7 languages**, on the web and on social media.

<a href="https://agentnewsie.live"><img src="https://img.shields.io/badge/📰_Read_the_news-agentnewsie.live-0EA5E9?style=for-the-badge" alt="Read the news at agentnewsie.live"/></a>
<a href="https://t.me/AgentNewsieTR"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"/></a>
<a href="https://instagram.com/agentnewsie"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"/></a>
<a href="https://threads.net/@agentnewsie"><img src="https://img.shields.io/badge/Threads-000?style=for-the-badge&logo=threads&logoColor=white" alt="Threads"/></a>

<img src="https://img.shields.io/website?url=https%3A%2F%2Fagentnewsie.live&style=flat-square&label=status&up_message=live&up_color=2ea44f" alt="live"/>
<img src="https://img.shields.io/badge/🇵🇱_PL_·_🇬🇧_EN_·_🇹🇷_TR_·_🇦🇿_AZ_·_🇰🇿_KK_·_🇰🇬_KY_·_🇺🇿_UZ-lightgrey?style=flat-square" alt="7 languages"/>

</div>

---

<table>
<tr>
<td width="55%" valign="top">

### Why Agent Newsie?

Living abroad means missing the news that matters to you: a new tax rule, a strike, a storm warning, a change at the immigration office. Local news is in Polish, and it is spread across dozens of sites.

Agent Newsie fixes that:

- 🕵️ **Reads for you:** watches Polish news sites and X 24/7
- ✍️ **Rewrites:** an LLM turns each story into a short, clear summary
- 🚨 **Ranks:** every story gets a criticality score, so breaking news goes first
- 🧹 **Filters:** duplicates, ads and repeat topics are dropped before they reach you
- 🌍 **Translates:** Polish, English, Turkish, Azerbaijani, Kazakh, Kyrgyz and Uzbek
- 📣 **Publishes:** to the website, Telegram, Instagram and Threads, with branded images
- 📅 **Events:** a local events page next to the news

</td>
<td width="45%" align="center" valign="middle">
<a href="https://agentnewsie.live"><img src="assets/demo.gif" width="100%" alt="Agent Newsie demo"/></a>
</td>
</tr>
</table>

## ⚙️ How it works

```mermaid
flowchart LR
    A[Polish news sites<br/>+ X search] -->|RSS · HTTP · Selenium| B[Ingestion]
    B --> C[Dedup & ad filter<br/>embeddings + story judge]
    C --> D[LLM rewrite<br/>+ criticality score]
    D --> E[Translate<br/>7 languages]
    E --> F[Watermarked<br/>media]
    F --> G[agentnewsie.live]
    F --> H[Telegram]
    F --> I[Instagram]
    F --> J[Threads]
```

## 📢 Advertise with Agent Newsie

Reach a multilingual community living in Poland, on the website and across social channels.

| 1. Design | 2. Pay | 3. Review | 4. Live |
|---|---|---|---|
| Pick your placements and preview your ad on every channel. | Secure checkout with Stripe. | Our team checks every ad before it runs. | Your ad appears on the site and goes out on social. |

Formats: website banner, social posts, reels and stories, booked by the day for up to 7 days, starting **from 7 PLN**.

<p align="center"><a href="https://agentnewsie.live"><img src="https://img.shields.io/badge/Book_an_ad_→-111827?style=for-the-badge" alt="Book an ad"/></a></p>

## 🛠️ Under the hood

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white" alt="Selenium"/>
  <img src="https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs" alt="Next.js"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white" alt="Raspberry Pi"/>
</p>

- **Python pipeline** built on Strategy + Factory: every fetcher, parser, LLM provider and publisher is a plug-in
- **LLM cascade:** Anthropic Claude, Google Gemini and Groq, with OpenAI moderation
- **Semantic dedup** with FastEmbed embeddings, a story judge and topic cooldowns
- **Next.js** public site, operator dashboard and self-serve advertiser flow
- Runs **24/7 on a Raspberry Pi** (ARM, CPU-only, Docker)

---

<div align="center">

<sub>This repository is the public home of Agent Newsie: updates and feedback. The source code is private.</sub>

<sub>Found a bug or want to suggest a news source? <a href="../../issues">Open an issue</a>.</sub>

<sub>Built by <a href="https://github.com/bbuyukyuksel">Burak Büyükyüksel</a>.</sub>

</div>
