# 🥽 AZ-305: Azure Messaging Services — Deep Dive

### Study Notes Repository — 2026 Edition

[![Deploy to GitHub Pages](https://github.com/marcogrimaldi29/az-305-messaging/actions/workflows/pages.yml/badge.svg)](https://github.com/marcogrimaldi29/az-305-messaging/actions/workflows/pages.yml)
[![GitHub Pages Live](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?logo=github)](https://marcogrimaldi29.com/az-305-messaging/)
[![Personal Hub of Marco Grimaldi](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)
[![AZ-305 Main Notes](https://img.shields.io/badge/AZ--305-Main%20Notes-blue?logo=microsoftazure)](https://marcogrimaldi29.com/az-305-study-notes/)

> - 🎯 **Goal:** Master the four Azure Messaging services for the **AZ-305: Designing Microsoft Azure Infrastructure Solutions** exam  
> - 📅 **Notes Version:** 2026  
> - 🌐 **Published site:** [🥽 AZ-305: Azure Messaging Services — Deep Dive](https://marcogrimaldi29.com/az-305-messaging/)  
> - ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)  
> - 🔗 **Companion repos:** [📘 AZ-305 Study Notes](https://marcogrimaldi29.com/az-305-study-notes/) · [🥽 AZ-305: Azure Compute Services — Deep Dive](https://marcogrimaldi29.com/az-305-compute/) · [🥽 AZ-305: Data & Analytics Services — Deep Dive](https://marcogrimaldi29.com/az-305-data-analytics/) · [🥽 AZ-305: Migration, HA & BCDR — Deep Dive](https://marcogrimaldi29.com/az-305-bcdr/) · [📘 AZ-104 Study Notes](https://marcogrimaldi29.com/az-104-study-notes/)


---

## 📋 Services Covered

| Service | Pattern | Key Use Case |
|---------|---------|--------------|
| 📨 **Azure Service Bus** | Message queue / pub-sub | Enterprise messaging, ordered delivery, transactions |
| 📦 **Azure Storage Queues** | Simple queue | Lightweight decoupling, large backlogs, low cost |
| 🏁 **Azure Event Grid** | Event routing (push) | React to state changes, serverless triggers |
| 🟩 **Azure Event Hubs** | Event streaming | High-throughput telemetry, log aggregation, Kafka |

---

## 🗂️ Repository Structure

```
az-305-messaging/
├── README.md                        ← 📍 You are here
├── index.md                         ← Site home page
├── 01-service-bus.md                ← Azure Service Bus deep dive
├── 02-storage-queues.md             ← Azure Storage Queues deep dive
├── 03-event-grid.md                 ← Azure Event Grid deep dive
├── 04-event-hubs.md                 ← Azure Event Hubs deep dive
├── 05-feature-comparison.md         ← Side-by-side comparisons & decision tables
└── 06-exam-caveats-cheatsheet.md    ← Exam traps, decision tree, quick-fire facts
```

---

## 🔑 Why This Exists

Messaging services are among the **most comparison-heavy topics** on the AZ-305 exam. The exam doesn't just ask what each service does — it presents scenarios where multiple services are plausible and asks which is the **best fit given constraints** such as:

- Ordering guarantees required?
- Message replay / retention needed?
- Millions of events per second?
- Dead-letter queue support?
- Transactions across multiple queues?
- Cost-sensitive simple decoupling?

This repository gives you the precise differentiators to answer those questions with confidence.

---

## 📚 Official Learning Resources

| Resource | Link |
|----------|------|
| 📄 Official AZ-305 Exam Page | [AZ-305 Exam](https://learn.microsoft.com/en-us/credentials/certifications/exams/az-305/) |
| 📋 Skills Measured / Study Guide | [Official Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-305) |
| 📨 Azure Service Bus Docs | [Service Bus Overview](https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-messaging-overview) |
| 📦 Storage Queues Docs | [Storage Queues Overview](https://learn.microsoft.com/en-us/azure/storage/queues/storage-queues-introduction) |
| 🏁 Event Grid Docs | [Event Grid Overview](https://learn.microsoft.com/en-us/azure/event-grid/overview) |
| 🟩 Event Hubs Docs | [Event Hubs Overview](https://learn.microsoft.com/en-us/azure/event-hubs/event-hubs-about) |
| 🧪 Free Practice Assessment | [Practice Assessment](https://learn.microsoft.com/en-us/credentials/certifications/exams/az-305/practice/assessment?assessment-type=practice&assessmentId=15) |

---

## ✅ Key Study Tips for Messaging Questions

- 🎯 Know the **exact message/event size limits** — they appear in scenario questions
- 🔄 Distinguish **"message"** (queue, guaranteed once) from **"event"** (notification, no payload)
- 💰 Know when **Storage Queues beat Service Bus** on cost/simplicity
- 📐 Know the **Event Grid vs Event Hubs** distinction: routing vs streaming
- ⚡ Memorise **throughput units, partitions, retention days** for Event Hubs
- 🔐 Know which features require **Service Bus Premium** (VNet, Geo-DR, sessions at scale)
- 📊 SLA values for each service appear in availability scenario questions

---

## 🌐 Published Website

This deep dive is hosted on **GitHub Pages** and published as a searchable website:

👉 **[🥽 AZ-305: Azure Messaging Services — Deep Dive](https://marcogrimaldi29.com/az-305-messaging/)**

The site includes full-text search, Mermaid diagram rendering, and mobile-friendly navigation.

These notes are designed to be a structured, exam-focused summary of the most important concepts and services baseds on the official [Microsoft AZ-305 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-305) and its criteria.

Additional study notes maintained by me are also available for those pursuing Microsoft and Azure certifications at the following Landing Page:

👉 **[🛬 Landing Page: Study Notes](https://marcogrimaldi29.com/study-notes/)**

---

## ✍️ About the Author

These notes are maintained by **[Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/){:target="_blank"}** — Cloud Consultant, Language Trainer & Lifelong Learner.

📍 **Find more content at [🌐 marcogrimaldi29.com](https://marcogrimaldi29.com){:target="_blank"}**

> The website is continuously updated and based on my personal study notes and experiences. If you have any feedback, suggestions, or corrections, feel free to [reach out](https://marcogrimaldi29.com/contact/){:target="_blank"}!

---

## 📈 Analytics

This site uses **[Umami](https://umami.is/)** for privacy-friendly analytics.

---

## © Credits & Acknowledgements

The **[Just the Docs](https://github.com/just-the-docs/just-the-docs)** theme is used for a clean, documentation-style layout. Licensed under [MIT](https://opensource.org/license/MIT).

Created with the help of AI. Model used: **[Claude Sonnet 4.6](https://www.anthropic.com/news/claude-sonnet-4-6)**. The content has been reviewed and edited by the author for accuracy and clarity, but may contain errors. Always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/azure/).

> *Not affiliated with or endorsed by Microsoft.*