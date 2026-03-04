---
layout: home
title: Home
nav_order: 1
---

# 📨 AZ-305: Azure Messaging Services — Deep Dive
{: .no_toc }

**Study Notes & Exam Prep — 2026 Edition**
{: .fs-5 .fw-300 }

[![Deploy to GitHub Pages](https://github.com/marcogrimaldi29/az-305-messaging/actions/workflows/pages.yml/badge.svg)](https://github.com/marcogrimaldi29/az-305-messaging/actions/workflows/pages.yml)
[![Personal Hub of Marco Grimaldi](https://img.shields.io/badge/Blog-marcogrimaldi29.com-blue?logo=rss)](https://marcogrimaldi29.com)
[![AZ-305 Study Notes](https://img.shields.io/badge/AZ--305-Study%20Notes-blue?logo=microsoftazure)](https://marcogrimaldi29.com/az-305-study-notes/)

> 🎯 **Purpose:** Deep-dive study notes covering the four core Azure Messaging services tested in the **AZ-305: Designing Microsoft Azure Infrastructure Solutions** exam.  
> 📅 **Version:** 2026  
> ✍️ **Author:** [Marco Grimaldi](https://www.linkedin.com/in/marco-grimaldi29/)  
> 🌐 **Published:** [marcogrimaldi29.com/az-305-messaging](https://marcogrimaldi29.com/az-305-messaging/)
> 🔗 **Companion repos:** [📘 AZ-305 Study Notes](https://marcogrimaldi29.com/az-305-study-notes/) · [🥽 AZ-305: Azure Messaging Services — Deep Dive](https://marcogrimaldi29.com/az-305-messaging/)

---

## 🗺️ What's in This Repository?

This companion repository to the [AZ-305 Study Notes](https://marcogrimaldi29.com/az-305-study-notes/) zooms into **Azure Messaging** — one of the most comparison-heavy topic clusters on the exam — with the depth needed to answer *"which service and why?"* questions confidently.

| File | Coverage |
|------|----------|
| [📨 01 — Azure Service Bus](01-service-bus.md) | Queues, Topics, Sessions, Dead-lettering, SKUs, SLAs |
| [📦 02 — Azure Storage Queues](02-storage-queues.md) | AT-LEAST-ONCE, visibility timeout, limits, integration |
| [⚡ 03 — Azure Event Grid](03-event-grid.md) | Event routing, topics, domains, filters, delivery |
| [🌊 04 — Azure Event Hubs](04-event-hubs.md) | Partitions, consumer groups, Capture, Kafka, SKUs |
| [📊 05 — Feature Comparison](05-feature-comparison.md) | Side-by-side tables: delivery, ordering, replay, limits |
| [🎯 06 — Exam Caveats & Cheatsheet](06-exam-caveats-cheatsheet.md) | Decision trees, exam traps, quick-fire facts |

---

## 🔑 Why Messaging Matters for AZ-305

Messaging patterns surface across **various exam domains**:

- **Data Storage:** choosing Storage Queues vs Service Bus for decoupling
- **Infrastructure Solutions:** event-driven architecture with Event Grid; high-throughput ingestion with Event Hubs
- **Business Continuity:** geo-disaster recovery for Service Bus Premium; Event Hubs Geo-DR
- **Well-Architected Framework:** reliability through async messaging; cost optimisation via tier selection

> ⚠️ The exam frequently presents **scenario-based questions** where multiple services *could* work — knowing the precise differentiators (message size limits, ordering guarantees, replay capability, dead-letter support) is what separates a correct answer from a plausible distractor.

---

## ⚡ Quick Navigation

| I need to know… | Go to |
|-----------------|-------|
| When to use Service Bus vs Storage Queues | [05 — Feature Comparison § Queues](05-feature-comparison.md#queues-service-bus-vs-storage-queues) |
| When to use Event Grid vs Event Hubs | [05 — Feature Comparison § Events](05-feature-comparison.md#events-event-grid-vs-event-hubs) |
| All four services side by side | [05 — Feature Comparison](05-feature-comparison.md) |
| Last-minute exam traps & decision tree | [06 — Exam Caveats](06-exam-caveats-cheatsheet.md) |
| Service Bus SKU differences | [01 — Service Bus § SKUs](01-service-bus.md#sku-tiers) |
| Event Hubs throughput units & partitions | [04 — Event Hubs § Capacity](04-event-hubs.md#capacity-model) |

---

*Not affiliated with or endorsed by Microsoft. Always verify against the latest [Microsoft documentation](https://learn.microsoft.com/en-us/azure/). Content is based on the [AZ-305 official study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-305).*
