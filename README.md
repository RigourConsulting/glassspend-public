# GlassSpend Public Information Website

**Repository:** `https://github.com/RigourConsulting/glassspend-public`  
**Official Public Website:** `https://rigourconsulting.github.io/glassspend-public/`  
**Application:** GlassSpend (Android)  
**Tagline:** See right through your bills.  
**Publisher:** Rigour Consulting Pty Ltd (Melbourne VIC, Australia)

---

## 1. Purpose of this Repository

This repository contains the authoritative, static HTML public information website for **GlassSpend**, an independent Australian personal cost organisation and bill management application.

It hosts required consumer transparency documents, legal policies, data deletion guides, and support resources for Australian consumers and the Google Play Store.

> [!CAUTION]
> **Strict Governance Warning for Maintainers:**  
> This is a public repository. Under no circumstances should private Android source code, keystores, signing keys, API credentials, customer documents, test fixtures, or personal financial data be committed or pushed to this repository.

---

## 2. Product Description

GlassSpend helps Australians organise bills, understand recurring costs, track due dates, and stay informed about changes in what they pay.

- **On-Device Optical Character Recognition (OCR):** Local Latin text recognition processing photos and PDFs without cloud document transmission.
- **Local-First Architecture:** Stored locally in a private Android Room SQLite database without compulsory cloud account registration.
- **Deterministic Mathematics:** Bill comparisons and change explanations formulated using exact integer cents calculations.
- **No Automatic Switching & No Commissions:** GlassSpend never accepts retailer bounties, never switches contracts automatically, and never requests internet banking credentials.

---

## 3. Public Website Structure

The site is built with lightweight, semantic HTML5 and vanilla CSS (WCAG 2.2 Level AA and AAA compliant) with zero runtime CDN dependencies:

```
/
├── index.html                  # Consumer landing page & feature overview
├── privacy.html                # Privacy Policy (Australian Privacy Principles)
├── terms.html                  # Terms of Service (Australian Consumer Law)
├── support.html                # Customer Support, FAQ, and troubleshooting
├── subscription-help.html      # GlassSpend Pro membership, Play billing & cancellation
├── delete-data.html            # Data deletion disclosures & request procedures
├── how-comparisons-work.html   # Comparison methodology, AER data & maths formulas
├── security.html               # Security architecture & threat model disclosures
├── accessibility.html          # Accessibility statement (WCAG 2.2 AA)
├── release-notes.html          # Public version release notes (v0.1.0)
├── 404.html                    # Branded 404 error page
├── robots.txt                  # Search engine crawler directives
├── sitemap.xml                 # Search engine XML sitemap
├── .nojekyll                   # Disables Jekyll processing for raw static files
└── assets/
    ├── css/
    │   └── style.css           # Central stylesheet with GlassSpend brand tokens
    └── img/
        ├── glassspend_icon.png # Official approved GlassSpend brand icon
        └── icon.svg            # Fallback vector icon
```

---

## 4. GitHub Pages Deployment Method

This site is deployed to GitHub Pages directly from the `main` branch.

### Configuration Settings
- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/(root)`
- **Published URL:** `https://rigourconsulting.github.io/glassspend-public/`

### Maintenance Instructions
1. Edit HTML/CSS files locally.
2. Run link checker and editorial audit scripts:
   ```bash
   python scripts/audit_website.py
   python scripts/check_website_links.py
   ```
3. Commit changes with clear, descriptive commit messages adhering to Australian English editorial standards.
4. Push to `origin main`.
5. Verify live deployment at `https://rigourconsulting.github.io/glassspend-public/`.

---

## 5. Contact & Support

- **General & Technical Support:** `support@rigourconsulting.com.au`
- **Privacy & Data Protection:** `privacy@rigourconsulting.com.au`
- **Engineering Security:** `security@rigourconsulting.com.au`
- **Accessibility Inquiries:** `accessibility@rigourconsulting.com.au`
- **Publisher:** Rigour Consulting Pty Ltd, Level 14, 380 Bourke Street, Melbourne VIC 3000, Australia
