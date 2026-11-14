# Security Policy

The AZ-305 Messaging Services Deep Dive is a static site built with Jekyll and the Just the Docs theme, and published to GitHub Pages by a GitHub Actions workflow. It has no accounts and no sign-in, search runs entirely in your browser, and the site sets no cookies and stores nothing on your device. Analytics are cookieless, through [Umami](https://umami.is/). Diagrams are drawn with Mermaid, loaded from the jsDelivr CDN, and the home page shows badge images from shields.io. The attack surface is small, but security reports are still welcome, and I'd rather hear about a problem privately before it's public.

---

## 🛡️ Supported Versions

There are no releases. Only what's live is maintained.

| Version | Supported |
| --- | --- |
| The live site at [marcogrimaldi29.com/az-305-messaging](https://marcogrimaldi29.com/az-305-messaging/) and the `main` branch | ✅ |
| Older commits, forks and copies hosted elsewhere | ❌ |

## 📮 Reporting a Vulnerability

**Please don't open a public issue or comment.** Instead, report it privately through GitHub: open the repo's **Security** tab and choose **Report a vulnerability**, or go straight to the [private report form](https://github.com/marcogrimaldi29/az-305-messaging/security/advisories/new). Only you and I can see the report, and we can discuss and fix the problem there before anything is made public.

It helps to include:

- The affected URL or file in this repo
- What the problem is and what someone could do with it
- The steps to reproduce it, or a short proof of concept

Please don't include real secrets, credentials or anyone else's personal data in the report, and don't test against anything that isn't yours.

If you can't use GitHub, send me a private message on [LinkedIn](https://www.linkedin.com/in/marco-grimaldi29/) instead, starting it with **"Security: AZ-305 Messaging Deep Dive"** so it's easy to spot.

## 🎯 Scope

**In scope:**

- The published site, including its pages, scripts and assets
- This repository's source, including the Jekyll configuration, includes and styles, and its GitHub Actions workflow
- A dependency version used here that has a known vulnerability, such as the theme, a Ruby gem, the Mermaid version or a GitHub Action

**Out of scope:**

- **Azure Service Bus, Queue Storage, Event Grid, Event Hubs or any other Microsoft product.** Report these to the [Microsoft Security Response Center](https://msrc.microsoft.com/create-report).
- **Apache Kafka or another open-source project the notes describe.** Report it through that project's own security process, such as [Apache Kafka project security](https://kafka.apache.org/community/project_security/).
- **A vulnerability in Jekyll, Just the Docs, Mermaid, Lunr or another dependency itself.** Report it to that project. If this repo uses an affected version, let me know as well.
- **HTTP response headers set by GitHub Pages.** The repo can't change them.
- **Automated scanner output** with no demonstrated impact on this site.
- **An insecure recommendation in the notes**, such as a design that relies on connection strings or shared access signatures where Microsoft Entra ID and a managed identity would do, or that leaves a namespace open to the internet when the scenario calls for private endpoints. That's a content issue, so it's welcome as a public issue — see the [contributing guide](CONTRIBUTING.md).

## ⏱️ What to Expect

I maintain this repo on my own, so responses are best effort. I'll confirm I've received your report, keep you posted in the private report while I look into it, and let you know when it's fixed. If you'd like to be credited, say so and I'll credit you in the security advisory or the fix.

Dependabot alerts and security updates are turned on for this repo, so known vulnerabilities in its dependencies are usually flagged and patched without a report.
