# Awesome-Rapid-Application-Development-Rad

# Awesome Rapid Application Development (RAD)

> A curated list of top Rapid Application Development (RAD) platforms — both SaaS/Hosted commercial low-code and no-code builders and open-source alternatives for visually assembling internal tools, admin panels, and business applications with minimal hand-coding.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Retool](#retool)
  - [Bubble](#bubble)
  - [OutSystems](#outsystems)
  - [Mendix](#mendix)
  - [Appian](#appian)
  - [FlutterFlow](#flutterflow)
  - [Zoho AppCreator](#zoho-appcreator)
- [Open-Source Software](#-open-source-software)
  - [ToolJet](#tooljet)
  - [Appsmith](#appsmith)
  - [Budibase](#budibase)
  - [Windmill](#windmill)
  - [Saltcorn](#saltcorn)
  - [Baserow](#baserow)
  - [Directus](#directus)
  - [DashPress](#dashpress)
  - [A12](#a12)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Rapid Application Development platforms. These are not open-source but are included as reference points for feature comparison.

### Retool
**Type:** Low-code platform for internal tools and admin panels
Retool is the most widely recognized commercial low-code platform for building internal tools, connecting to databases and APIs with a drag-and-drop UI builder. It includes AI credits for assisted development. Pricing starts at $10/month per builder for the Team plan, with a free tier for small teams [citation:6]. It is the benchmark against which open-source alternatives like ToolJet and Appsmith are measured.

### Bubble
**Type:** No-code full-stack web application builder
Bubble is a leading no-code platform for building full web applications, with visual logic and a hosted database. It is positioned for founders and non-technical builders creating SaaS products, marketplaces, and web apps. Pricing starts at $59/month (billed annually) for the Starter plan, with a free tier available [citation:6]. Its strength is the breadth of what can be built without code; the trade-off is potential vendor lock-in and performance ceilings at scale.

### OutSystems
**Type:** Enterprise low-code platform
OutSystems is a long-standing enterprise low-code platform for building web and mobile applications with visual modeling, full-stack capabilities, and deployment automation. It is known for enterprise governance, lifecycle management, and integration depth. Pricing is quote-based and typically targets mid-to-large enterprises.

### Mendix
**Type:** Enterprise low-code with model-driven development
Mendix (Siemens) provides a visual development environment with model-driven architecture, multi-cloud deployment, and strong governance features. It supports collaborative development between business users and IT. Pricing is quote-based with a free tier for small teams.

### Appian
**Type:** Low-code automation with process orchestration
Appian's low-code platform combines visual app design with process automation, case management, and AI capabilities. It is strong in regulated industries needing audit trails and compliance controls. Pricing is quote-based.

### FlutterFlow
**Type:** Visual Flutter app builder
FlutterFlow is a visual app builder that generates real Flutter code, letting teams design and build mobile and web apps through a drag-and-drop interface while keeping access to the underlying, exportable codebase. It has a free plan with up to 2 projects, and paid plans from $39/month for unlimited projects and code export [citation:6]. It is the go-to choice for teams wanting native mobile apps without writing Flutter by hand.

### Zoho AppCreator
**Type:** No-code app builder within Zoho ecosystem
Zoho AppCreator (part of Zoho Creator) provides a no-code environment for building business applications with forms, workflows, and reports. It is the natural choice for organizations already using Zoho products, with tight integration into the broader Zoho suite.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Rapid Application Development tools. The open-source ecosystem is strongest for **internal tools and admin panels**, with several mature platforms competing directly with Retool.

### ToolJet
**Stack:** Node.js / React / PostgreSQL | **License:** GPL-3.0 (Community) / AGPL-3.0 (self-hosted)
ToolJet is an extensible low-code framework for building and deploying internal tools with minimal engineering effort, positioned as an alternative to Retool and Mendix . Key features include a drag-and-drop interface with **40+ pre-built UI components**, **30+ database connectors** (PostgreSQL, MySQL, MongoDB), REST API and GraphQL integration, real-time data synchronization, a visual query builder, workflow designer, form builder, and multi-user collaboration with role-based permissions . It is **one of the healthiest open-source projects** in this category, with a Repoly health score of 98/100, 41k GitHub stars, and 1,421 commits in 90 days [citation:10]. It offers a **permanent cloud free plan** (2 builders, 50 end users, 2 apps, 100 AI credits/month) and a fully open-source community edition for unlimited self-hosted users [citation:13]. **Caveat:** The self-hosted edition's AGPL licensing means distributing a modified ToolJet as a product requires open-sourcing your changes [citation:13].  
**Best for:** Teams wanting the most feature-dense open-source Retool alternative with strong health metrics and a generous free tier, accepting copyleft licensing for self-hosted distribution.

### Appsmith
**Stack:** Java / React / MongoDB | **License:** Apache-2.0
Appsmith is an open-source framework to build admin panels, CRUD apps, and workflows, positioned as a Retool alternative. It has **41k GitHub stars**, a Repoly health score of **98/100**, and **1,896 commits in 90 days** — the most raw commit activity among the top open-source alternatives [citation:10]. Its **Apache-2.0 license is permissive**, allowing forking or embedding without publishing changes [citation:10]. It offers a cloud free plan and paid plans from $15/user/month (Business) [citation:6]. It is the strongest choice for teams that need permissive licensing or plan to embed the builder into their own product.  
**Best for:** Teams prioritizing a permissive license and high development velocity for internal tools, particularly those wanting to embed or customize without copyleft obligations.

### Budibase
**Stack:** Node.js / Svelte | **License:** GPL-3.0 (Open Source) / Proprietary (Enterprise)
Budibase is an open-source low-code platform for building, automating, and shipping internal tools on your own infrastructure, positioned as an alternative to OutSystems, Retool, Mendix, and Appian [citation:10]. It includes a built-in database plus connectors for Postgres, MySQL, MongoDB, Airtable, and REST APIs, with an automation engine for scheduled jobs and multi-step workflows [citation:13]. The **self-hosted edition is free forever under GPLv3** with no per-seat or per-app license fee [citation:13]. **Important caveat:** Its cloud free tier has been limited to 5 users and ~200 monthly automation runs, and **Repoly reports its current license as Proprietary/source-available rather than pure open source** [citation:10], so verify licensing terms carefully for your use case.  
**Best for:** Teams wanting an accessible, all-in-one open-source internal tool builder with built-in automation, verifying current licensing before deployment.

### Windmill
**Stack:** Rust / Go / TypeScript / PostgreSQL | **License:** AGPLv3 (Community)
Windmill is an open-source developer platform that turns scripts into webhooks, workflows, and UIs, positioned as an **open-source alternative to Retool and Temporal** [citation:2][citation:14]. It is a **code-first** platform: you write scripts in Python, TypeScript, Go, or Bash, and Windmill automatically generates a UI from the script's parameters. It claims to be the **fastest workflow engine (13x vs Airflow)** [citation:2]. It has 12,931 GitHub stars and active development (latest release 4 days ago) [citation:2]. The community edition is free for internal use under AGPLv3 . **Trade-off:** It is less of a drag-and-drop builder than ToolJet or Appsmith—teams comfortable writing code will get the most value.  
**Best for:** Developer teams wanting to turn existing scripts into internal UIs and workflows with a fast, code-first platform, accepting AGPL terms.

### Saltcorn
**Stack:** Node.js / PostgreSQL | **License:** MIT
Saltcorn is an open-source no-code application builder with a focus on **self-hosting simplicity**—it can run on a **2 GB VPS** and installs via a simple `npx saltcorn-install -y` command on Linux [citation:5]. It provides a drag-and-drop UI builder, data views, and a plugin ecosystem. It is positioned for users wanting a straightforward, self-hosted no-code platform without the complexity of enterprise tools. **Trade-off:** Less feature-dense than ToolJet or Appsmith, with a smaller community.  
**Best for:** Individuals and small teams wanting a lightweight, MIT-licensed no-code builder they can run on minimal infrastructure.

### Baserow
**Stack:** Python / Django / Vue.js / PostgreSQL | **License:** MIT (Open Source Edition) / Proprietary (Premium)
Baserow is an open-source no-code database and application builder, positioned as an Airtable alternative. The **Application Builder** removes its beta label in version 2.4.1 and is now declared production-ready [citation:12]. It provides a spreadsheet-like interface with 20+ field types, forms, and automations. The **Open Source Edition is MIT-licensed**, with premium features under a separate commercial license. Self-hosting uses an all-in-one Docker image that bundles PostgreSQL, Redis, and Caddy [citation:12]. It is a strong choice if your primary need is a structured data layer with a simple app UI on top.  
**Best for:** Teams wanting an open-source Airtable alternative with a production-ready application builder, accepting that it is database-first rather than a full drag-and-drop tool builder.

### Directus
**Stack:** Node.js / Vue.js / SQL | **License:** BUSL-1.1 (source-available)
Directus wraps any SQL database with a realtime GraphQL+REST API and an intuitive admin app for non-technical users, positioned as an instant App & API for your database [citation:10]. It has 39k GitHub stars and a health score of 98/100 [citation:10]. **Important licensing caveat:** It is **BUSL-1.1 (source-available, not OSI-approved)**, which limits commercial reuse [citation:10]. It is best suited for teams that already have a database schema and want a powerful admin UI and API layer without building from scratch.  
**Best for:** Teams with existing SQL databases wanting an instant admin app and API, accepting the source-available licensing terms.

### DashPress
**Stack:** TypeScript / Node.js | **License:** Open Source
DashPress lets you generate powerful admin apps without writing a single line of code—running `npx dashpress` scaffolds an admin interface from your database [citation:1]. It is positioned for rapid admin panel generation rather than full application building. It is listed among open-source internal tool frameworks [citation:1].  
**Best for:** Developers wanting to instantly generate an admin panel from an existing database schema with minimal setup.

### A12
**Stack:** Java / Model-driven | **License:** EUPL 1.2 (Community Edition)
A12 is a German open-source platform for model-driven development of enterprise applications, underpinning major public sector systems including Germany's federal tax portal ELSTER (50+ million tax returns annually) [citation:7]. It strengthens **digital sovereignty in Europe**, allowing organizations to understand, control, and adapt critical software independently [citation:7]. It is released under the **EUPL 1.2** on openCode and GitHub. **Trade-off:** It is enterprise and public-sector focused, with a model-driven approach that differs from typical drag-and-drop low-code tools.  
**Best for:** European public sector organizations and enterprises prioritizing digital sovereignty and model-driven development, accepting a steeper learning curve than consumer-grade builders.

---

## 📊 Comparison at a Glance

| Software | License | Stack | UI Builder | Database | Self-Hosted | Best For |
|----------|---------|-------|------------|----------|-------------|----------|
| **Retool** | Proprietary | Cloud | ✅ Drag-and-drop | ✅ Connectors | ❌ | Commercial internal tools |
| **Bubble** | Proprietary | Cloud | ✅ Drag-and-drop | ✅ Hosted | ❌ | Full no-code web apps |
| **OutSystems** | Proprietary | Cloud | ✅ Visual | ✅ | ❌ | Enterprise low-code |
| **FlutterFlow** | Proprietary | Cloud | ✅ Drag-and-drop | (Firebase) | ❌ | Native mobile apps |
| **ToolJet** | GPL/AGPL | Node.js/React | ✅ 40+ components | ✅ 30+ connectors | ✅ | Feature-dense OSS Retool alt |
| **Appsmith** | Apache-2.0 | Java/React | ✅ Drag-and-drop | ✅ | ✅ | Permissive OSS + embed |
| **Budibase** | GPL-3.0 | Node.js/Svelte | ✅ | ✅ Built-in | ✅ | All-in-one OSS + automation |
| **Windmill** | AGPLv3 | Rust/Go/TS | (Script-generated) | ✅ PostgreSQL | ✅ | Code-first scripts → UIs |
| **Saltcorn** | MIT | Node.js/Postgres | ✅ Drag-and-drop | ✅ PostgreSQL | ✅ | Lightweight self-hosted |
| **Baserow** | MIT (OSS) | Python/Vue | ✅ App Builder | ✅ Built-in | ✅ | Database-first app builder |
| **Directus** | BUSL-1.1 | Node.js/Vue | ✅ Admin app | ✅ Any SQL | ✅ | Instant API + admin on SQL |
| **A12** | EUPL 1.2 | Java | ✅ Model-driven | (Check) | ✅ | European sovereignty + enterprise |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Rapid Application Development (RAD) tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with Directus and Baserow's premium tiers). Note that the open-source ecosystem for **internal tools and admin panels** is very mature, with **ToolJet** and **Appsmith** leading on health and community metrics [citation:10]. **Appsmith** is the strongest choice if a permissive license matters , while **ToolJet** offers the densest feature set with a generous cloud free tier [citation:13]. **Windmill** takes a fundamentally different, code-first approach for developer teams [citation:2]. For full no-code web applications (Bubble-style), open-source options are thinner—**Baserow** and **Directus** are database-first rather than application-first.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
