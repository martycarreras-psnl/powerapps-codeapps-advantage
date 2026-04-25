# Power Apps Code Apps Advantage

A single-page strategic brief making the enterprise case for **Microsoft Power Platform Code Apps with Dataverse** over Lovable and bespoke React-on-Azure-SQL approaches — especially at scale (10,000 users, ~1,000 makers) and in regulated industries handling PHI.

> **One platform. Fewer moving parts. Greater value.**

---

## What's in this repo

| Path | Purpose |
|------|---------|
| `index.html` | The deployed GitHub Pages site. References images from `/images`. Lightweight (~46 KB). |
| `assets/code-apps-vs-lovable-embedded.html` | A fully self-contained version with all images embedded as base64 data URIs (~13 MB). Open it directly from disk, email it, or drop it on a SharePoint site — no external dependencies. |
| `images/` | Source PNG visuals used by `index.html`. Web-friendly filenames. |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing and serve the files as-is. |

---

## Sections of the brief

1. **Persona Maturity Model** — Business Innovator → Citizen Developer → Professional Developer → Final Governed Application. Often the same human across all four roles.
2. **Governance & ALM at Scale** — Configure Managed Environments once, let 1,000 makers self-serve.
3. **Compliance & Data Residency** — The deciding factor for PHI: Code Apps inside the customer's Azure tenant under a signed Microsoft BAA, vs Lovable on Supabase / AWS where the Terms & Conditions and DPA explicitly prohibit PHI.
4. **MCP Server Advantage** — Dataverse exposes tables, relationships, and security to agents natively; Azure SQL does not.
5. **Power Pages BYOC** — External-facing React SPAs for users outside Entra ID, with the same Dataverse security posture.
6. **Dataverse vs Azure SQL** — Deep capability comparison.
7. **True Total Cost of Ownership** — Cost complexity, not dollar figures: few components vs many components, one bill vs many bills.
8. **AI Flexibility & Model Transparency** — Bring any frontier model (Claude, GPT-5, Gemini 2.5, Cursor, Grok, DeepSeek, Qwen) and always know which one you're running.
9. **Strategic Conclusion** — For governed, compliant, agent-ready scale, Code Apps with Dataverse is the clear winner.

---

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In **Settings → Pages**, set the source to **Deploy from a branch**, branch **main**, folder **/ (root)**.
3. After the first build, the brief will be live at:
   `https://<your-org>.github.io/power-apps-code-apps-advantage/`

The `.nojekyll` file ensures GitHub Pages serves files exactly as committed (no Jekyll processing of underscores, etc.).

---

## Local preview

```bash
# Either open index.html directly in a browser…
open index.html

# …or serve the folder with any static file server:
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

## Distributing the standalone version

When you need a single-file, link-free, offline-safe copy (email attachments, executive briefings, customers without internet), use:

```
assets/code-apps-vs-lovable-embedded.html
```

Every image is embedded as base64, so the file renders identically with no external dependencies.

---

*The AI coding tool is just the hammer. The platform is the house.*
