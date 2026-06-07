# GapFew

> A multi-framework compliance **gap self-assessment** — score your coverage and see the few gaps that matter.

GapFew is part of the **Few** toolkit, alongside the rest of the suite (see the full list below). Like the others, it is a single, free, fully client-side HTML page: nothing you enter ever leaves your browser.

🔗 **Live:** https://silvestroparisi.github.io/GapFew/

---

## What it is

"Are we compliant?" is rarely a yes/no. GapFew turns it into something you can actually work with: a structured, control-by-control self-assessment that shows where you stand and, above all, **which gaps to close first**.

You rate each control as **implemented**, **partial**, **not implemented** or **N/A**, with a short note recording your evidence. Each control comes with concrete ✗ / ◐ / ✓ examples so the rating isn't guesswork, and a live scorecard tracks your coverage as you go.

## The frameworks

GapFew covers four frameworks, **289 controls** in total, in Italian and English:

- **NIS2** — 49 controls, based on the technical measures of Commission Implementing Regulation **(EU) 2024/2690**
- **NIST CSF 2.0** — 106 controls across the six functions (Govern, Identify, Protect, Detect, Respond, Recover)
- **ISO/IEC 27001:2022** — 93 Annex A controls
- **GDPR** — 41 controls across principles, lawful basis, rights, security, breaches, transfers and governance

## How it works

1. **Pick a framework** and fill in your organization header (org, assessor, date).
2. **Rate each control** — the ✗ / ◐ / ✓ examples show what each level looks like in practice.
3. **Record evidence** in the *Evidence* field for each control — what you've actually implemented. This is what feeds a remediation plan later.
4. **Watch the scorecard** — coverage is computed as implemented = 1, partial = 0.5, not implemented = 0; N/A and unanswered are excluded.
5. **Export** — save/load your work as JSON, export a CSV, or print to PDF. The PDF and CSV are **prioritized**: the gaps to address first (not-implemented, then partial) are listed before the full table.

Click **Demo** to load a worked example for the active framework (an example SME), so you can see a completed assessment immediately.

## Privacy

100% client-side. There is no backend, no account, no analytics. Your assessment lives only in the page until you save it. Don't take my word for it — it's open source, and you can watch the Network tab: nothing is sent.

## What GapFew is — and isn't

**GapFew is a self-assessment and orientation tool. It is not an audit, a certification, or a legal opinion.** It helps you see and prioritize gaps; it does not certify compliance. A few honest caveats:

- **ISO/IEC 27001** Annex A control text is copyrighted by ISO. GapFew paraphrases each control in plain language for self-assessment; it is not a reproduction of the standard, which you should obtain to implement an ISMS properly.
- **GDPR** compliance is highly context-dependent. Whether a control applies, and how, depends on your specific processing, roles and risk — and ultimately on legal interpretation. Treat the result as a starting map, not advice.
- **NIS2**: the technical measures in CIR (EU) 2024/2690 are legally binding only for the specific types of digital-infrastructure entities the regulation lists (DNS, cloud, data centres, managed services, marketplaces, etc.). Other essential/important entities follow their national transposition — in Italy, **D.Lgs. 138/2024** and the guidance of **ACN**. GapFew uses these measures as a practical, widely applicable baseline, not as a statement of what legally binds *you*.

For anything that matters, validate with a qualified assessor, DPO or lawyer.

## Companion: CloseFew

GapFew finds the gaps; **[CloseFew](https://silvestroparisi.github.io/CloseFew/)** turns them into a plan. Export your assessment as JSON, load it into CloseFew, and an AI of your choice walks each control with you and drafts what to do to become compliant.

## Deploy it yourself

1. Create a repository named `GapFew`.
2. Add `index.html` (this single file) to the root.
3. Enable GitHub Pages (Settings → Pages → deploy from the `main` branch, root).
4. It's live at `https://<your-username>.github.io/GapFew/`.

## The Few toolkit

- [**FirstFew**](https://silvestroparisi.github.io/FirstFew/) — prioritize the few that matter
- [**FixFew**](https://silvestroparisi.github.io/FixFew/) — verify and remediate vulnerabilities
- [**MaskFew**](https://silvestroparisi.github.io/MaskFew/) — anonymize a file before you share it
- [**AskFew**](https://silvestroparisi.github.io/AskFew/) — a private AI that runs in your browser
- [**ScrubFew**](https://silvestroparisi.github.io/ScrubFew/) — strip hidden metadata before you share
- [**RopaFew**](https://silvestroparisi.github.io/RopaFew/) — build your GDPR Article 30 register
- **GapFew** — a multi-framework compliance gap self-assessment
- [**CloseFew**](https://silvestroparisi.github.io/CloseFew/) — turn your gaps into a remediation plan
