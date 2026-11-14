# Contributing to the AZ-305 Messaging Services Deep Dive

Thanks for helping keep these notes accurate. They're a deep dive into the messaging topics of **Microsoft Exam AZ-305: Designing Microsoft Azure Infrastructure Solutions**, covering Azure Service Bus, Azure Storage Queues, Azure Event Grid and Azure Event Hubs. Azure changes fast: features move between tiers, size limits and retention periods change, and preview features become generally available between one revision of the study guide and the next. Reports from people studying with the notes are the best way to catch that.

> [!IMPORTANT]
> **This repo accepts issues, not pull requests.** Pull requests are turned off: I write every change myself and check it against the official documentation, so the notes keep one voice and stay consistent with the main AZ-305 notes and the other deep dives. If you know exactly how something should read, put your proposed wording in the issue. It's just as useful.

---

## Contents

- [Ways to Help](#-ways-to-help)
- [Before You Open an Issue](#-before-you-open-an-issue)
- [Opening an Issue](#-opening-an-issue)
- [Out of Scope](#-out-of-scope)
- [What Happens Next](#-what-happens-next)
- [Code of Conduct](#-code-of-conduct)
- [Security](#-security)

## 🙌 Ways to Help

Every report fits one of the six types in the issue template:

| Type | What it covers | For example |
| --- | --- | --- |
| **Content error** | Text, a table, a callout, a Mermaid diagram or a number such as an SLA, a size limit or a retention period is wrong | A figure in the SLA Comparison doesn't match the tier it's listed against, or the decision tree sends a scenario that needs a dead-letter queue to the wrong service |
| **Outdated content** | An Azure service, tier, feature or limit, or the exam, has changed since the page was written | A feature the notes keep to Premium is now in Standard, a figure in Must-Memorise Numbers has changed, or a preview feature is now generally available |
| **Exam coverage** | The notes don't match the official study guide | The study guide was revised after April 17, 2026, or *Recommend a messaging architecture* or *Recommend an event-driven architecture* isn't covered in enough depth |
| **Site bug** | Search, navigation, Mermaid diagrams, a broken link or accessibility | The decision tree on the cheatsheet page doesn't render, a Table of Contents link lands on the wrong section, or a link returns 404 |
| **Device issue** | Something looks wrong or doesn't work on a specific device, browser or screen size | The Master Comparison Table can't be scrolled sideways on a phone, or the navigation menu won't open on a tablet |
| **Suggestion** | Something could be clearer or easier to study | A topic that would read better as a comparison table or a diagram, another scenario for a Common Exam Scenarios table, or another trap for the exam caveats cheatsheet |

## 🔎 Before You Open an Issue

- **Search the existing issues**, [open and closed](https://github.com/marcogrimaldi29/az-305-messaging/issues?q=is%3Aissue). If yours is already there, add a 👍 reaction or a comment with anything new rather than opening a duplicate.
- **Check the date.** The notes follow the **skills measured as of April 17, 2026**, mainly *Recommend a messaging architecture* and *Recommend an event-driven architecture* under *Design an application architecture*. If the "Skills measured as of" heading in the [AZ-305 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-305) shows a newer date, say so in the issue — it tells me which revision to compare against.
- **Check the current docs.** A quick look at the documentation for [Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/), [Queue Storage](https://learn.microsoft.com/en-us/azure/storage/queues/), [Event Grid](https://learn.microsoft.com/en-us/azure/event-grid/) or [Event Hubs](https://learn.microsoft.com/en-us/azure/event-hubs/) usually confirms whether something has changed, and gives you the link the issue asks for. For a comparison or decision table, Microsoft's guides to [choosing between Event Grid, Event Hubs and Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/compare-messaging-services) and to [Storage queues and Service Bus queues](https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-azure-and-service-bus-queues-compared-contrasted) are a good place to start.
- **One problem per issue.** Separate issues are easier to track, fix and close. Several typos on the same page can go in one issue.
- **For a site bug, hard-refresh first** (Ctrl+F5, or Cmd+Shift+R on a Mac) in case your browser is showing an older copy of the page.

## 📝 Opening an Issue

1. Open a new issue with the [🐞 Report an Issue](https://github.com/marcogrimaldi29/az-305-messaging/issues/new?template=ISSUE_TEMPLATE.md) template.
2. Give it a title that names the page and the problem, for example *"04 — Azure Event Hubs: SKU Tiers table gives an old retention limit"* rather than *"Mistake on page"*.
3. Fill in the template's sections. Leave out any that don't apply.

> [!TIP]
> To link straight to a section, click it in the page's **Table of Contents**, or hover over its heading and click the link icon, then copy the address from your browser.

### What Makes a Report Easy to Fix

- **A link to the exact section**, not just the page
- **The text as the notes have it**, quoted, so it can be found even if the page has moved on
- **An official source** for any content change — Microsoft Learn is best. For a number such as a size limit, a retention period or a quota, or for a feature that needs a particular tier, link the page that states it, and for an SLA, Microsoft's [Service Level Agreements (SLA) for Online Services](https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services). A report without a source may take longer, because every change has to be checked against the documentation before it goes in
- **For bugs and device issues:** the steps to reproduce it, what you expected and what happened instead, the device, operating system and browser, and a screenshot if it shows the problem
- **Your proposed wording**, if you have it. With pull requests turned off, this is the closest thing to suggesting an edit directly

## 🚫 Out of Scope

To keep the notes accurate and the issue tracker useful, please don't open issues for:

- **Live exam content.** Questions, answers or topics remembered from a real exam break [Microsoft's exam security policy](https://learn.microsoft.com/en-us/credentials/support/exam-and-assessment-lab-security-policies). Issues or comments that include them will be closed and the content removed.
- **Exam booking, scores or retakes.** [Microsoft Credentials support](https://learn.microsoft.com/en-us/credentials/support/help) can help with those.
- **Help with your own Azure environment.** For troubleshooting messages piling up in a dead-letter queue, an Event Grid subscription whose webhook won't validate, Event Hubs consumers that fall behind or a storage queue full of poison messages, ask on [Microsoft Q&A](https://learn.microsoft.com/en-us/answers/) or [open an Azure support request](https://learn.microsoft.com/en-us/azure/azure-portal/supportability/how-to-create-azure-support-request).
- **Anything private.** Issues are public, so leave out subscription and tenant IDs, namespace, topic and resource names, IP addresses, connection strings, SAS keys and tokens, storage account keys and customer details, including in screenshots.
- **Other AZ-305 topics.** This deep dive covers the four messaging services listed in the README. Services that send or process the messages are covered elsewhere: Azure Functions and Logic Apps in [Compute](https://github.com/marcogrimaldi29/az-305-compute), and Stream Analytics and IoT Hub in [Data & Analytics](https://github.com/marcogrimaldi29/az-305-data-analytics). For a mistake in those, in the [AZ-305 Study Notes](https://github.com/marcogrimaldi29/az-305-study-notes) or in the [Migration, HA & BCDR](https://github.com/marcogrimaldi29/az-305-bcdr) deep dive, open the issue on that repo instead.
- **Unofficial sources.** Practice-test sites, exam dump sites and AI chat answers aren't accepted as the source for a content change.
- **Promotion.** Links to courses, products or services, affiliate links and paid placements won't be added.
- **Security vulnerabilities.** Please [report these privately](https://github.com/marcogrimaldi29/az-305-messaging/security/advisories/new), as described in the [security policy](SECURITY.md), not in a public issue.

## 🔄 What Happens Next

- I maintain the notes on my own, in my spare time, so replies are best effort and there's no fixed response time.
- I check each report against the official documentation. If something needs clarifying, I'll ask on the issue, so keep an eye on your GitHub notifications.
- When a fix goes in, the issue is closed with a note or a link to the change. The live site updates shortly after.
- If nothing changes, the issue is closed with the reason, such as out of scope, can't be verified, or working as intended.
- An issue waiting on a reply may be closed after a while. Comment with the missing details and it can be reopened.

## 🤝 Code of Conduct

By opening, commenting on or reacting to issues here, you agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md). Comments that are abusive, spam or share live exam content may be hidden, edited or locked.

## 🔒 Security

Found a security problem with the site or this repo? Please don't report it in a public issue. Use [Report a vulnerability](https://github.com/marcogrimaldi29/az-305-messaging/security/advisories/new) instead, so only you and I can see it. The [security policy](SECURITY.md) has the details.

---

If the notes helped you, the README's [💚 Support](https://github.com/marcogrimaldi29/az-305-messaging#-support) section has a couple of ways to show it. Thanks for helping make them better for the next AZ-305 candidate.
