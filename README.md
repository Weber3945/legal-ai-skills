# Set Up an AI-Powered Full-Service Law Firm in 90 Seconds

To install **Legal AI Skills by Rohas Nagpal**, open **Claude Code** or the **Codex** app or CLI on your computer and run this prompt. It does not install in Codex on the web (chatgpt.com/codex) or in a claude.ai chat.

```text
Install Legal AI Skills from https://github.com/rohasnagpal/legal-ai-skills and say "Hello Rohas".
```
---
<img width="949" height="799" alt="image" src="https://github.com/user-attachments/assets/1ab803f3-7578-4e67-85f2-a8dead314202" />

## Here's What You Get

- **1 Managing Partner:** Receives matters, assigns specialist lawyers, coordinates work and reviews final outputs.

- **17 Specialist Lawyers:** Handle matters across practice areas such as corporate, criminal defence, contracts, family law, real estate, tax and litigation.

- **3 Jurisdiction Counsel:** Identify and verify applicable laws, legal authorities and procedures in India, the US and the UK.

- **226 Legal Skills:** Reusable capabilities such as contract review, legal research, due diligence, evidence analysis and legal drafting, including jurisdiction-specific skills for RERA and Section 138 NI Act.

- **20 Workflows:** Step-by-step processes for matters such as M&A due diligence, divorce proceedings, contract negotiation and litigation preparation.

- **14 Official Legal Research Sources and Connectors:** Provide access to legislation, regulations, judgments, court records, official notices, company registries and sanctions lists through official and authoritative legal sources.

- **Built-in Legal Tools:** Exact deadline and interest calculators, and private sanctions screening against the US, UK and UN lists, all running on your own machine.

Built in India 🇮🇳 for the world by [Rohas Nagpal](https://rohasnagpal.com/).

---

## Should I Sue?

Facing a dispute and not sure whether to pursue it? Install with this prompt instead:

```text
Install Legal AI Skills from https://github.com/rohasnagpal/legal-ai-skills and say "Should I Sue".
```

Put your contracts, emails, messages, screenshots and notices in one folder, open a new session in that folder, and ask **"Should I sue?"** A team of AI lawyers reads every document, examines the claims, evidence, risks, costs, chances and alternatives, and recommends litigation, arbitration, mediation, negotiation, a regulatory or consumer complaint, or walking away, with any urgent deadline first. It reads only the folder you open, and the final decision is yours. More at [docs/should-i-sue.md](docs/should-i-sue.md).

---

## How It Works

1. **Managing Partner** receives the matter and consults Jurisdiction Counsel to identify applicable laws, jurisdiction, relevant procedures and required expertise.

2. **Managing Partner** assigns the most appropriate Specialist Lawyer as Matter Owner and selects a relevant workflow, where available.

3. **Matter Owner** develops a matter plan, identifies the required skills, adapts the workflow to the case and delegates tasks to other Specialist Lawyers as needed. The Matter Owner remains responsible for coordinating the matter throughout.

4. **Specialist Lawyers** conduct research, analysis, drafting and review using relevant legal skills. Jurisdiction Counsel provides and verifies applicable local laws, procedures and legal authorities.

5. **Matter Owner** consolidates findings, resolves inconsistencies, identifies outstanding issues and prepares the final deliverables.

6. **Managing Partner** reviews the completed work for completeness, legal reasoning, consistency, supporting evidence, verified authorities and legal risks. Jurisdiction Counsel assists with final local-law verification where required. The Managing Partner requests revisions when necessary.

7. **Final output** is delivered to the user, clearly identifying any unresolved issues, unverified information and required human legal review or approval.

Simple questions skip the team: the Managing Partner uses the one relevant skill directly.

---

## Architecture

```text
AI Managing Partner
│
├── Jurisdiction Counsel
│   ├── India Counsel
│   ├── US Counsel
│   └── UK Counsel
│
├── Specialist Lawyers
│   ├── Corporate Lawyer
│   ├── Contracts Lawyer
│   ├── Litigation Lawyer
│   ├── Dispute Resolution Lawyer
│   ├── Criminal Defence Lawyer
│   ├── Family Lawyer
│   ├── Real Estate Lawyer
│   ├── Tax Lawyer
│   ├── Insolvency Lawyer
│   ├── Banking & Finance Lawyer
│   ├── Employment Lawyer
│   ├── Intellectual Property Lawyer
│   ├── Compliance Lawyer
│   ├── Consumer Protection Lawyer
│   ├── Public Law & Regulatory Lawyer
│   ├── Investigations Lawyer
│   └── Legal Research Lawyer
│
├── Legal Skills
│   ├── Jurisdiction-Neutral Skills
│   └── Jurisdiction-Specific Skills
│
├── Matter Workflows
│   ├── M&A Due Diligence
│   ├── Contract Review & Negotiation
│   ├── Litigation Preparation
│   ├── Divorce Proceedings
│   ├── RERA Complaints
│   └── ...
│
├── Official Legal Research Sources & Connectors (14)
│   ├── Legislation & Regulations — legislation.gov.uk, eCFR, Federal Register, GovInfo
│   ├── Case Law & Judgments — CourtListener, Find Case Law
│   ├── Court, Rulemaking & Official Notices — CourtListener dockets, Regulations.gov, The Gazette
│   ├── Company Registries — SEC EDGAR, GLEIF, UK Companies House
│   └── Sanctions Lists — US OFAC, UK Sanctions List, UN Consolidated List
│
└── Built-in Legal Tools (run on your machine)
    ├── Deadline & Interest Calculators — deadlines, periods between dates, simple & compound interest
    ├── Sanctions Screening — private, alias-aware name screening
    └── Document Production — DOCX, PDF, conversion, OCR & bundle assembly
```

---

## Important Considerations

**Confidentiality:** Before uploading client documents or confidential information, ensure that your AI environment and connected services comply with applicable confidentiality, privacy and professional obligations.

**Human Review:** AI-generated legal analysis, advice and documents should be reviewed by an appropriately qualified legal professional where required. Court filings, representation and other regulated legal activities remain subject to applicable professional and legal requirements.

**Legal Accuracy:** The system should verify applicable laws and authorities wherever possible and clearly disclose any information it cannot verify. Its outputs are not guaranteed to be accurate or complete.

---

## For AI Assistants Installing This

If you are Codex or Claude running the install prompt above, follow [AGENTS.md](AGENTS.md). In short:

- **Claude Code:** run `claude plugin marketplace add rohasnagpal/legal-ai-skills`, then `claude plugin install legal-ai-skills@rohas-legal` in the terminal yourself. (A person can type `/plugin marketplace add …` and `/plugin install …` instead.)
- **Codex:** run `codex plugin marketplace add rohasnagpal/legal-ai-skills`, then `codex plugin add legal-ai-skills@rohas-legal`.
- Confirm the plugin appears in the installed plugins list, then print the post-install message in [AGENTS.md](AGENTS.md). The new skills load in a new session or after `/reload-plugins`, so tell the user to do that and then type **Hello Rohas**.

Node.js 18 or later is needed for the bundled registry, research and document tools. The legal skills work without it.

**Upgrading from vCLO:** the plugin is now `legal-ai-skills`. Uninstall the older Rohas plugins (`vclo-by-rohas`, `rohas-legal-ai`, `navigator`, `privacy`) and install `legal-ai-skills@rohas-legal`, so skills and connectors don't load twice. In the Codex desktop app, quit and reopen the app after installing so the connectors load. "Hello vCLO" still works for this release.

---

## Updating to a New Version

Paste this into Claude Code or Codex:

```text
Update Legal AI Skills from https://github.com/rohasnagpal/legal-ai-skills
```

Or run the commands yourself:

```bash
# Claude Code
claude plugin marketplace update rohas-legal
claude plugin update legal-ai-skills@rohas-legal

# Codex
codex plugin marketplace upgrade rohas-legal
codex plugin add legal-ai-skills@rohas-legal
```

Then restart: in Claude Code run `/reload-plugins` or start a new session; in Codex start a new chat, and in the Codex desktop app quit and reopen it. Say **Hello Rohas** to check the version is working. See the [changelog](CHANGELOG.md) for what changed.

---

## The 20 Workflows

| Workflow | Matter Owner |
|---|---|
| [Divorce and matrimonial proceedings](plugins/legal-ai-skills/workflows/divorce-and-matrimonial-proceedings.md) | Family Lawyer |
| [RERA complaint](plugins/legal-ai-skills/workflows/rera-complaint.md) | Real Estate Lawyer |
| [Property purchase due diligence](plugins/legal-ai-skills/workflows/property-purchase-due-diligence.md) | Real Estate Lawyer |
| [Cheque dishonour (Section 138)](plugins/legal-ai-skills/workflows/cheque-dishonour.md) | Litigation or Criminal Defence Lawyer |
| [Criminal defence](plugins/legal-ai-skills/workflows/criminal-defence.md) | Criminal Defence Lawyer |
| [Consumer complaint](plugins/legal-ai-skills/workflows/consumer-complaint.md) | Consumer Protection Lawyer |
| [Tax assessment and appeal](plugins/legal-ai-skills/workflows/tax-assessment-and-appeal.md) | Tax Lawyer |
| [Insolvency and CIRP](plugins/legal-ai-skills/workflows/insolvency-cirp.md) | Insolvency Lawyer |
| [Debt recovery](plugins/legal-ai-skills/workflows/debt-recovery.md) | Banking & Finance Lawyer |
| [Employment dispute](plugins/legal-ai-skills/workflows/employment-dispute.md) | Employment Lawyer |
| [Contract review and negotiation](plugins/legal-ai-skills/workflows/contract-review-and-negotiation.md) | Contracts Lawyer |
| [M&A due diligence](plugins/legal-ai-skills/workflows/m-and-a-due-diligence.md) | Corporate Lawyer |
| [Financing transaction](plugins/legal-ai-skills/workflows/financing-transaction.md) | Banking & Finance Lawyer |
| [Dispute viability assessment](plugins/legal-ai-skills/workflows/dispute-viability-assessment.md) | Litigation Lawyer |
| [Litigation preparation](plugins/legal-ai-skills/workflows/litigation-preparation.md) | Litigation Lawyer |
| [Commercial dispute lifecycle](plugins/legal-ai-skills/workflows/commercial-dispute-lifecycle.md) | Litigation Lawyer |
| [Arbitration lifecycle](plugins/legal-ai-skills/workflows/arbitration-lifecycle.md) | Dispute Resolution Lawyer |
| [Regulatory compliance review](plugins/legal-ai-skills/workflows/regulatory-compliance-review.md) | Compliance Lawyer |
| [Data breach response](plugins/legal-ai-skills/workflows/data-breach-response.md) | Compliance Lawyer |
| [Internal investigation](plugins/legal-ai-skills/workflows/internal-investigation.md) | Investigations Lawyer |

Each workflow names its Matter Owner, supporting lawyers, branches, review checkpoints and escalation points.

---

## Research Sources, Connectors and Tools

| Source | Coverage | Access |
|---|---|---|
| CourtListener | US case law and court records | Free account |
| GovInfo | US federal statutes, regulations and records | Free API key recommended |
| eCFR (Code of Federal Regulations) | US federal regulations, current or as at a date | No account |
| Federal Register | US rules and notices | No account |
| Regulations.gov | US rulemaking dockets | Free API key |
| legislation.gov.uk | UK legislation | No account |
| Find Case Law (The National Archives) | UK judgments | No account |
| The Gazette | UK insolvency, company and probate notices | No account; rate-limited |
| SEC EDGAR | US company filings | No account |
| GLEIF | Global legal entity identifiers | No account |
| UK Companies House | UK company records | Free key may be needed |
| US OFAC sanctions lists (SDN and consolidated) | US sanctions designations and aliases | No account; screened locally |
| UK Sanctions List | UK sanctions designations and aliases | No account; screened locally |
| UN Security Council Consolidated List | UN sanctions designations and aliases | No account; screened locally |

India Counsel routes Indian research through official sources such as India Code, eGazette, the Supreme Court, High Courts, tribunals and regulators where accessible. There is no unrestricted eCourts access, paid database or commercial citator. When a source is unavailable, the firm says what it could not check.

**Sanctions screening:** the firm downloads the official US, UK and UN sanctions lists, keeps them on your machine for 24 hours, and screens names there with fuzzy matching across aliases, so the names you screen are never sent to anyone. Results are potential matches for review, not clearance, and EU, Indian and other national lists are not included. See the [sanctions screening guide](plugins/legal-ai-skills/integrations/sanctions-screening.md).

**Legal calculators:** a local, offline calculator ([guide](plugins/legal-ai-skills/integrations/legal-calculators.md)) computes deadlines (days, working days, months or years, with supplied holidays), periods between dates, and simple or compound interest, exactly and with the working shown. It applies only the rules it is given, so statutory periods and rates still come from Jurisdiction Counsel.

The firm also includes a local document-production adapter for DOCX and PDF creation, conversion, OCR and assembly using free local engines, and can use documents, email, calendars and cloud storage that you connect and authorise in your host.

---

## See It in Action

Start with the [two-minute guide](docs/two-minute-start.md), then see fictional demonstrations for an [Indian divorce](examples/india-divorce.md), a [RERA complaint](examples/rera-complaint.md), [contract negotiation](examples/contract-review-and-negotiation.md), [M&A due diligence](examples/m-and-a-due-diligence.md), an [Indian commercial dispute](examples/india-commercial-dispute.md), [US privacy applicability](examples/us-privacy-applicability.md) and a [UK employment issue](examples/uk-employment-issue.md).

---

## Sample Prompts

1. Two founders are splitting equity 60/40. Draft a founders' agreement with four-year vesting, a one-year cliff and IP assignment to the company.

2. A UK employer wants to dismiss a remote worker after a failed performance review. What must be established before we can give advice?

3. A customer bought a defective laptop online and the seller refuses to replace it. Can they file a consumer complaint in India, and what compensation can they claim?

4. An employee has reported that her manager is harassing her. As the company, what should we do under India's POSH Act, step by step?

5. We want to launch an online marketplace for customers in California, Texas and New York. Which US state privacy laws might apply, and what facts do we need to confirm?

6. Draft a mutual NDA between two Indian companies exploring a joint venture, with a two-year confidentiality period and arbitration in Mumbai.

---

## FAQ

**Is my client data sent anywhere?** Your documents stay in your Codex or Claude environment. The calculators and sanctions screening run on your machine; research connectors send only the search terms needed to the official source. Check your own AI provider's data terms before sharing confidential material.

**Where does it run?** Inside Codex or Claude. In Claude Code each lawyer runs as its own subagent. In Codex, lawyers run as subagents where Codex supports it, or their work is performed in turn and kept separate.

**What does it cost?** $0, plus your ChatGPT or Claude subscription.

**Who is it for?** Practising lawyers, in-house counsel, startups, businesses and law students.

**Languages?** It works in the languages your Codex or Claude model supports. The skills and source guides are maintained in English, so verify translations, defined terms and filing-language requirements.

**For law firms:** need help setting up or customising Legal AI Skills? Contact [Rohas Nagpal](https://rohasnagpal.com) at rohasnagpal@gmail.com.

---

# The Lawyers and Their Skills

Each skill is listed under the lawyer who owns it. Many are shared: any lawyer can use any skill, and the [skill registry](plugins/legal-ai-skills/skill-registry.yaml) records the owner, shared users and jurisdiction of every skill. Jurisdiction-specific skills are marked 🇮🇳, 🇺🇸 or 🇬🇧.

[Managing Partner and firm operations](#managing-partner-and-firm-operations) · [Corporate Lawyer](#corporate-lawyer) · [Contracts Lawyer](#contracts-lawyer) · [Litigation Lawyer](#litigation-lawyer) · [Dispute Resolution Lawyer](#dispute-resolution-lawyer) · [Criminal Defence Lawyer](#criminal-defence-lawyer) · [Family Lawyer](#family-lawyer) · [Real Estate Lawyer](#real-estate-lawyer) · [Tax Lawyer](#tax-lawyer) · [Insolvency Lawyer](#insolvency-lawyer) · [Banking and Finance Lawyer](#banking-and-finance-lawyer) · [Employment Lawyer](#employment-lawyer) · [IP Lawyer](#ip-lawyer) · [Compliance Lawyer](#compliance-lawyer) · [Consumer Protection Lawyer](#consumer-protection-lawyer) · [Public Law and Regulatory Lawyer](#public-law-and-regulatory-lawyer) · [Investigations Lawyer](#investigations-lawyer) · [Legal Research Lawyer](#legal-research-lawyer) · [India Counsel](#india-counsel) · [US Counsel](#us-counsel) · [UK Counsel](#uk-counsel)

### Managing Partner and firm operations

Instructions: [managing-partner.md](plugins/legal-ai-skills/agents/managing-partner.md)

- **[adversarial-reviewer](plugins/legal-ai-skills/skills/adversarial-reviewer/SKILL.md)**: attacks your own draft the way opposing counsel would
- **[ask-vclo](plugins/legal-ai-skills/skills/ask-vclo/SKILL.md)**: Legacy name for Legal AI Skills by Rohas Nagpal
- **[assumption-flagger](plugins/legal-ai-skills/skills/assumption-flagger/SKILL.md)**: surfaces every assumption a draft depends on
- **[brief-to-counsel-drafter](plugins/legal-ai-skills/skills/brief-to-counsel-drafter/SKILL.md)**: focused instructions, facts, issues, record, questions and logistics
- **[client-intake](plugins/legal-ai-skills/skills/client-intake/SKILL.md)**: turns a messy client narrative into a structured matter summary, separating facts from assumptions
- **[client-update-drafter](plugins/legal-ai-skills/skills/client-update-drafter/SKILL.md)**: plain, honest status updates for a client on a running matter
- **[closure-report-drafter](plugins/legal-ai-skills/skills/closure-report-drafter/SKILL.md)**: controlled closure, client handoff, obligations, finances and retention
- **[conflict-checker](plugins/legal-ai-skills/skills/conflict-checker/SKILL.md)**: confidential party mapping, searches, escalation and clearance records
- **[consistency-checker](plugins/legal-ai-skills/skills/consistency-checker/SKILL.md)**: checks facts, dates, defined terms and figures across a document set
- **[costing-estimator](plugins/legal-ai-skills/skills/costing-estimator/SKILL.md)**: transparent stage budgets, scenarios, assumptions and change controls
- **[engagement-letter-drafter](plugins/legal-ai-skills/skills/engagement-letter-drafter/SKILL.md)**: scope, fees, exclusions and conflict position in a client engagement letter
- **[hello-rohas](plugins/legal-ai-skills/skills/hello-rohas/SKILL.md)**: Your AI law firm: Managing Partner, specialist lawyers and counsel
- **[issue-spotter](plugins/legal-ai-skills/skills/issue-spotter/SKILL.md)**: reads a fact pattern for issues, causes of action and threshold problems
- **[learn-law-with-rohas](plugins/legal-ai-skills/skills/learn-law-with-rohas/SKILL.md)**: interactive legal tutor — structured lessons, hypotheticals, quizzes, adaptive difficulty and a final assessment on a law or topic of your choice
- **[legal-document-producer](plugins/legal-ai-skills/skills/legal-document-producer/SKILL.md)**: template-aware DOCX and PDF production, conversion, OCR, assembly and final-format quality control
- **[legal-exam-prep-with-rohas](plugins/legal-ai-skills/skills/legal-exam-prep-with-rohas/SKILL.md)**: exam-focused revision — study plans, mock exams, adaptive quizzes, answer-structure coaching and weak-are