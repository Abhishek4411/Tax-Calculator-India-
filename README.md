# India Tax Regime Calculator — FY 2025–26

<div align="center">

╔══════════════════════════════════════════════════════════════╗  
║                                                              ║  
║     💰  SMART TAX CALCULATOR FOR FY 2025–26  💰             ║  
║                                                              ║  
║      Compare • Calculate • Save • Invest Smartly             ║  
║                                                              ║  
╚══════════════════════════════════════════════════════════════╝

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=for-the-badge)](#-changelog)  
[![License](https://img.shields.io/badge/license-MIT-green.svg?style=for-the-badge)](#-license)  
[![Tax Year](https://img.shields.io/badge/Tax%20Year-FY%202025--26-orange.svg?style=for-the-badge)](#-overview)  
[![Maintenance](https://img.shields.io/badge/Maintained-Yes-success.svg?style=for-the-badge)](#-roadmap)

**A zero‑dependency, privacy‑first tax calculator that runs entirely in your browser.**

[🚀 Quick Start](#-quick-start) • [📖 Documentation](#-documentation) • [🌟 Features](#-features) • [🛠️ Tech Stack](#-tech-stack)

</div>

---

## 📊 Overview

A comprehensive **single‑file** web application that helps Indian salaried employees make informed decisions between Old and New tax regimes for **FY 2025–26 (AY 2026–27)**. Built with vanilla JavaScript. No backend, no tracking, completely private.

### Why choose this calculator?

| Feature | Benefit |
|---|---|
| ✅ **Latest Rules** | Budget 2025 assumptions (rebate up to taxable ₹12.75 L, 30% top slab above ₹24 L) |
| ✅ **Comprehensive** | HRA, 80C, 80D, Home Loan, NPS, LTA & more |
| ✅ **Private** | 100% local calculations; zero data collection |
| ✅ **Free Forever** | No subscriptions, no ads, open source |
| ✅ **Professional** | CA‑style breakdowns and explanations |
| ✅ **Instant** | Real‑time calculations as you type |

> ⚠️ Always verify numbers against official sources before filing (see [Disclaimer](#-disclaimer)).

---

## 🌟 Features

```
INPUT → CALCULATE → RECOMMEND → VISUALIZE → EXPORT
```

<table>
<tr>
<td width="50%">

#### 🧮 Tax Engine
- Dual regime comparison (Old vs New)  
- HRA exemption (metro / non‑metro)  
- Home‑loan interest & principal  
- 80C / 80D / 80E deductions  
- NPS (employer + self 80CCD(1B))  
- LTA calculations  
- Cess & surcharge

</td>
<td width="50%">

#### 📈 Visual Analytics
- Tax vs Take‑home bar chart  
- Income distribution doughnut  
- Tax‑slab comparison graph  
- Animated rendering & legends  
- Export‑ready visuals

</td>
</tr>
<tr>
<td>

#### 📰 Live News Feed
- Auto‑scrolling ticker  
- Budget updates tab  
- Tax news & trends  
- Pause‑on‑hover  
- Time‑stamped items

</td>
<td>

#### 💰 Smart Recommendations
- Personalized investment tips  
- Tax‑saving quantification  
- 80C / 80D / NPS suggestions  
- Benefit limits tracking

</td>
</tr>
</table>

---

## 🎨 Tech Stack

### Architecture
```
┌─────────────────────────────────────────────┐
│          Single HTML File (~45 KB)          │
├─────────────────────────────────────────────┤
│  HTML5 │ CSS3 │ Vanilla JavaScript (ES6+)   │
├─────────────────────────────────────────────┤
│           Chart.js 4.4.x (CDN)              │
├─────────────────────────────────────────────┤
│        LocalStorage API (Persistence)       │
└─────────────────────────────────────────────┘
```

### Technology Breakdown

| Layer | Technology | Purpose | Version |
|---|---|---|---|
| **Structure** | HTML5 | Semantic markup | 5 |
| **Styling** | CSS3 | Animations & responsive layout | 3 |
| **Logic** | JavaScript | Tax engine & UI | ES6+ |
| **Charts** | Chart.js | Data visualization | 4.4.x |
| **Storage** | LocalStorage | Client‑side persistence | Web API |

### Color Scheme (CSS variables)
```css
:root {
  /* Primary */
  --primary: #2563eb;        /* Buttons, headers */
  --primary-dark: #1e40af;   /* Hover states */

  /* State */
  --success: #10b981;        /* Recommendations */
  --warning: #f59e0b;        /* Alerts, news */
  --danger:  #ef4444;        /* Critical info */

  /* Gradients */
  --gradient-primary: linear-gradient(135deg, #667eea, #764ba2);
  --gradient-success: linear-gradient(90deg, #10b981, #059669);
  --gradient-warning: linear-gradient(90deg, #fbbf24, #f59e0b);
}
```

### Animation Map
| Element | Animation | Duration |
|---|---|---|
| Cards | `fadeIn` | 0.6s |
| Results panel | `slideInRight` | 0.6s |
| Charts | `easeInOutQuart` | 2.0s |
| News Ticker | `ticker` (loop) | 60s |
| Buttons | `pulse` (infinite) | 2s |
| Progress bars | `shimmer` | 2s |

---

## 🚀 Quick Start

### Option 1: Direct clone (recommended)
```bash
git clone https://github.com/yourusername/india-tax-calculator.git
cd india-tax-calculator
# Open in your browser
open tax_calculator.html   # macOS
# or
xdg-open tax_calculator.html  # Linux
# or just double‑click the file in your file explorer
```

### Option 2: Single‑file download
```bash
# wget
wget https://raw.githubusercontent.com/yourusername/india-tax-calculator/main/tax_calculator.html

# curl
curl -O https://raw.githubusercontent.com/yourusername/india-tax-calculator/main/tax_calculator.html
```

### Option 3: GitHub Pages
1. Fork the repository  
2. **Settings → Pages**  
3. Select **main** branch → **Save**  
4. Access: `https://yourusername.github.io/india-tax-calculator/tax_calculator.html`

### System Requirements
- **Browser:** Chrome 90+, Firefox 88+, Safari 14+, Edge 90+  
- **Internet:** Only for first‑time Chart.js CDN fetch  
- **Storage:** ~100 KB LocalStorage  
- **JavaScript:** Must be enabled

---

## 💻 Usage Guide

### Step‑by‑step
1. **Enter income details**  
   - Annual CTC / Gross income  
   - Basic salary  
   - DA (if applicable)

2. **Add deductions (tick if applicable)**  
   - **HRA**: HRA received, rent paid, metro/non‑metro  
   - **Home Loan**: principal & interest, property type  
   - **80C**: EPF/VPF, PPF/ELSS/NSC, principal repayment  
   - **80D**: Health insurance (self/family + parents)  
   - **NPS**: Employer contribution; Self (80CCD(1B))  
   - **Others**: 80E (education loan interest), LTA

3. **Calculate** → click **Calculate Tax**

4. **Review**  
   - Regime recommendation  
   - Comparison cards & detailed breakdowns  
   - Visual charts  
   - Investment suggestions

5. **Export (optional)**  
   - Download CSV/Excel report  
   - Print formatted report

### Examples

<details>
<summary><b>Example 1: Fresh Graduate (₹8 L CTC)</b></summary>

```yaml
Input:
  CTC: ₹8,00,000
  Basic: ₹4,00,000
  HRA Received: ₹2,00,000
  Rent Paid: ₹2,40,000/year (Metro)
  EPF (80C): ₹48,000

New Regime:
  Gross: ₹8,00,000
  Standard Deduction: ₹75,000
  Taxable: ₹7,25,000
  Tax: ₹0 (rebate up to ₹12.75L)

Old Regime:
  Gross: ₹8,00,000
  Standard Deduction: ₹50,000
  HRA Exemption: ₹1,60,000
  80C: ₹48,000
  Taxable: ₹5,42,000
  Tax: ~₹2,100 + cess

Result:
  ✅ Recommended: NEW REGIME
  💰 Tax Savings: ~₹2,184
  🏠 Take‑home: ~₹8,00,000
```
</details>

<details>
<summary><b>Example 2: Mid‑career Professional (₹25 L CTC)</b></summary>

```yaml
Input:
  CTC: ₹25,00,000
  Basic: ₹12,50,000
  HRA Received: ₹5,00,000
  Rent Paid: ₹6,00,000/year (Metro)
  Home Loan Interest: ₹2,00,000
  80C (EPF + Others): ₹1,50,000
  80D: ₹50,000
  NPS Self (80CCD 1B): ₹50,000

New Regime (illustrative):
  Taxable Income: ₹24,25,000
  Tax: ₹4,16,250 + cess
  Total: ~₹4,32,900

Old Regime (illustrative):
  Deductions: ~₹8,75,000
  Taxable Income: ₹15,75,000
  Tax: ₹2,87,500 + cess
  Total: ~₹2,99,000

Result:
  ✅ Recommended: OLD REGIME
  💰 Tax Savings: ~₹1,33,900
  🏠 Take‑home: ~₹22,01,000
```
</details>

---

## 📖 Documentation

### Tax Slabs (FY 2025–26 — **assumptions reflecting Budget 2025**)

> These slabs reflect common interpretations used by popular calculators as of October 2025. Always verify with the official Finance Act / CBDT notifications before filing.

#### New Regime
| Income Range (₹) | Rate | Max tax on slab |
|---:|---:|---:|
| 0 – 4,00,000 | 0% | ₹0 |
| 4,00,001 – 8,00,000 | 5% | ₹20,000 |
| 8,00,001 – 12,00,000 | 10% | ₹40,000 |
| 12,00,001 – 16,00,000 | 15% | ₹60,000 |
| 16,00,001 – 20,00,000 | 20% | ₹80,000 |
| 20,00,001 – 24,00,000 | 25% | ₹1,00,000 |
| **Above 24,00,000** | **30%** | — |

- **Rebate:** Full tax waiver if **taxable income ≤ ₹12,75,000**  
- **Standard deduction:** **₹75,000**

#### Old Regime
| Income Range (₹) | Rate | Max tax on slab |
|---:|---:|---:|
| 0 – 2,50,000 | 0% | ₹0 |
| 2,50,001 – 5,00,000 | 5% | ₹12,500 |
| 5,00,001 – 10,00,000 | 20% | ₹1,00,000 |
| **Above 10,00,000** | **30%** | — |

- **Rebate:** Full tax waiver if **taxable income ≤ ₹5,00,000**  
- **Standard deduction:** **₹50,000**

> Health & Education Cess @ 4% applies; surcharge per prevailing thresholds.

### Key Formulas (Old vs New)

**HRA Exemption (Old only)**
```python
HRA_Exempt = min(
    actual_HRA_received,
    0.50 * (Basic + DA),               # Metro: Delhi/Mumbai/Kolkata/Chennai
    actual_rent_paid - 0.10 * (Basic + DA)
)
# For non-metro, replace 0.50 with 0.40
```

**Section 80C (Old only)**
```python
Total_80C = min(
    EPF + VPF + PPF + ELSS + NSC +
    Home_Loan_Principal +
    Life_Insurance_Premium +
    Tuition_Fees,
    150000
)
```

**Home Loan Interest — Section 24(b)**
```python
if property_type == "self_occupied":
    deduction = min(home_loan_interest, 200000)
elif property_type == "let_out":
    deduction = home_loan_interest  # No limit (subject to set-off rules)
```

**Section 80D (Old only)**
```python
# Self/Spouse/Children
self_family_limit = 25000    # < 60 years
self_family_limit = 50000    # ≥ 60 years

# Parents
parents_limit = 25000        # < 60 years
parents_limit = 50000        # ≥ 60 years

max_80D = 75000              # If all seniors
```

### Deduction Availability Matrix
| Deduction | Limit | Old Regime | New Regime | Notes |
|---|---:|:--:|:--:|---|
| **Standard Deduction** | ₹50K / ₹75K | ✅ | ✅ | Higher in New |
| **HRA Exemption** | Calculated | ✅ | ❌ | Old only |
| **80C (EPF/PPF/ELSS)** | ₹1.5L | ✅ | ❌ | Old only |
| **80D (Health Insurance)** | ₹25K–₹75K | ✅ | ❌ | Old only |
| **24(b) Home‑loan Interest** | ₹2L | ✅ | ⚠️ | New: Let‑out only |
| **NPS Employer** | 14% of Basic+DA | ✅ | ✅ | Both regimes |
| **80CCD(1B) NPS Self** | ₹50K | ✅ | ❌ | Old only |
| **80E (Education Loan)** | Interest only | ✅ | ❌ | Max 8 years |
| **LTA** | Actuals | ✅ | ❌ | Old only |
| **80G Donations** | 50–100% | ✅ | ❌ | Old only |

### Break‑Even (Illustrative)
| CTC Range | Old better if total deductions ≥ |
|---|---|
| ₹5–10 L | ₹1.5 L |
| ₹10–15 L | ₹3.5 L |
| ₹15–20 L | ₹5.5 L |
| ₹20–25 L | ₹7.5 L |
| ₹25–30 L | ₹8.0 L |
| ₹30 L+ | ₹8.0 L |

> These are approximations; actual outcomes depend on salary structure and specific deductions.

---

## 🔧 Technical Details

### File Structure
```
tax_calculator.html
└── <head>
    ├── <meta> (viewport, charset)
    ├── <title>
    └── <style> (variables, animations, grid, components, print)
└── <body>
    ├── Header
    ├── News Container (Ticker + Tabs)
    ├── Main Grid
    │   ├── Input Panel
    │   └── Results Panel (recommendation, comparison, details)
    └── <script>
        ├── Constants (Slabs, Limits)
        ├── Calculation functions
        ├── Chart.js integration
        ├── News management
        ├── LocalStorage handlers
        └── Export functions
```

### Key JavaScript Functions
```javascript
// Core
function calculateTax() {}                 // Main calculator
function calculateHRA() {}                 // HRA exemption
function calculateTaxOnSlabs(income, slabs) {}
function formatCurrency(amount) {}

// UI
function displayResults() {}
function populateTable(tableId, data) {}
function switchTab(index) {}
function switchNewsTab(index) {}

// Visualization
function createCharts() {}
function destroyCharts() {}

// Persistence
function saveData() {}
function loadData() {}

// Export
function downloadExcel() {}

// News
function initializeNews() {}
function loadNewsTab(tabId, articles) {}
```

### Browser Compatibility
| Browser | Version | Status | Notes |
|---|---:|:--:|---|
| Chrome | 90+ | ✅ | Recommended |
| Firefox | 88+ | ✅ | Full support |
| Safari | 14+ | ✅ | Desktop & iOS |
| Edge | 90+ | ✅ | Chromium‑based |
| Opera | 76+ | ✅ | Full support |
| Chrome Mobile | Latest | ✅ | Android |
| Safari Mobile | Latest | ✅ | iOS/iPadOS |

> Required: JavaScript enabled, LocalStorage enabled, Canvas support.

---

## 🔒 Privacy & Security

### Data Flow (100% local)
```
USER BROWSER
 ├─ Input Form
 ├─ JS Calculation Engine (local only)
 ├─ Results
 └─ LocalStorage (auto‑save)
```

- ❌ No server communication  
- ❌ No external API calls (except Chart.js CDN)  
- ❌ No cookies, no analytics  
- ✅ Works offline after initial load (Chart.js cached)  
- ✅ CSP‑friendly; no `innerHTML` with user input

---

## 🧪 Testing (Illustrative Coverage)

- **Income brackets:** ₹5L, ₹8L, ₹12L (rebate boundary), ₹15L, ₹20L, ₹25L, ₹30L, ₹50L, ₹75L, ₹1 Cr+  
- **HRA:** metro (50%), non‑metro (40%), no HRA, varied rents, edge cases  
- **Home loan:** self‑occupied (₹2L cap), let‑out (no cap), joint loan, interest‑only vs P+I  
- **80C combos:** EPF, PPF, ELSS, full ₹1.5L, overflow handling  
- **Edge cases:** zero income, negative inputs, very high income, all deductions maxed, slab boundaries  
- **UI/UX:** mobile/tablet layouts, print styles, chart rendering, animation performance, LS limits

---

## 🤝 Contributing

### Ways to contribute
1. 🐛 Report bugs  
2. 💡 Suggest features  
3. 📝 Improve docs  
4. 🎨 Enhance UI/UX  
5. 🧮 Verify calculations  
6. 🌐 Add translations  
7. 🔧 Submit code

### Dev workflow
```bash
# 1) Fork
# 2) Clone your fork
git clone https://github.com/YOUR_USERNAME/india-tax-calculator.git
cd india-tax-calculator

# 3) Feature branch
git checkout -b feature/your-feature-name
# e.g. feature/multi-language-support

# 4) Make changes (edit tax_calculator.html)

# 5) Test thoroughly (Chrome/Firefox/Safari, mobile, etc.)

# 6) Commit clearly
git add tax_calculator.html
git commit -m "Add: detailed description of change"

# 7) Push & open PR
git push origin feature/your-feature-name
```

#### Code Style
**HTML**
```html
<!-- ✅ Good: semantic, indented -->
<div class="input-group">
  <label for="ctc">Annual CTC</label>
  <input type="number" id="ctc" placeholder="2500000" />
</div>
```

**CSS**
```css
/* ✅ Good: organized, commented */
.card {
  background: var(--bg-white);
  border-radius: 16px;
  padding: 25px;
  box-shadow: var(--shadow-lg);
  transition: all 0.3s;
}
```

**JavaScript**
```javascript
// ✅ Good: clear, documented
function calculateHRA() {
  if (!document.getElementById('hasHRA').checked) return 0;

  const hraReceived = Number(document.getElementById('hraReceived').value) || 0;
  const rentPaid    = Number(document.getElementById('rentPaid').value) || 0;
  const basic       = Number(document.getElementById('basic').value) || 0;

  // Apply HRA formula...
}
```

**PR Checklist**
- Style & conventions followed  
- Calculations verified with examples  
- Tested on Chrome, Firefox, Safari  
- Mobile responsive preserved  
- No console errors/warnings  
- Comments for complex logic  
- README updated if needed  
- No breaking changes  
- LocalStorage compatibility intact  
- Charts render correctly

---

## 🗺️ Roadmap

**v1.1 (Q1 2026)**  
- Dark mode toggle  
- Multi‑year comparison (FY 2024–25 vs 2025–26)  
- Salary restructuring suggestions  
- PDF export (rich)  
- PWA support

**v1.5 (Q2 2026)**  
- Hindi language support  
- 5‑year tax projection  
- Form‑16 analyzer/parser  
- Advanced planning scenarios  
- Previous‑year comparison

**v2.0 (Q3 2026)**  
- Sections 54/54F (capital gains)  
- Freelancer/business income support  
- TDS/advance tax planning  
- Multi‑source income handling  
- Regional languages (Tamil/Telugu/Bengali)

**v2.5 (Q4 2026)**  
- Voice input  
- AI‑powered optimizations  
- Mobile app (React Native)  
- Offline‑first architecture  
- Encrypted cloud backup (opt‑in)

---

## 📝 Changelog

### **1.0.0** — October 2025
- Initial release  
- Old vs New regime comparison engine  
- Deductions: HRA, Home loan (24b + 80C principal), 80C, 80D, NPS (employer + self 80CCD(1B)), 80E, LTA  
- Chart.js visualizations (3 types)  
- Live news ticker & tabs  
- Investment recommendations  
- Auto‑save via LocalStorage  
- CSV/Excel export, print‑optimized layout  
- Responsive design & smooth animations  
- Comprehensive documentation

---

## ⚠️ Disclaimer

> **FOR EDUCATIONAL & ESTIMATION PURPOSES ONLY**  
> This calculator provides tax **estimates** based on standard rules as of **FY 2025–26**.
>
> - ❌ Not professional tax advice  
> - ❌ Not for official filing (ITR)  
> - ❌ Doesn’t cover every edge case  
> - ✅ Use for planning/learning/regime comparison
>
> **Consult a Chartered Accountant** for official filing, complex cases, legal advice, or disputes. The developer assumes **no liability** for financial decisions made using this tool.

### Scope & Limitations
**Covers:** salaried income, standard deductions/exemptions, HRA, 80C/80D/24b/80E/LTA/NPS, regime comparison, basic investment suggestions.  
**Does NOT cover:** business/professional income (complex), capital gains, certain “other sources”, agricultural/foreign income & DTAA, trusts/HUF, Section 54/54F, TDS/TCS, advance tax scheduling, complex perquisites.

---

## 📚 Resources

### Official
- Income Tax Dept: `incometax.gov.in`  
- Union Budget Docs: `indiabudget.gov.in`  
- Finance Act: `egazette.nic.in`  
- CBDT Circulars: `incometaxindia.gov.in`

### Learning
- ClearTax — Planning articles  
- Economic Times Tax — News  
- Moneycontrol Tax — Calculators  
- LiveMint Money — Personal finance

### Calculators (for cross‑checks)
- Income Tax Dept (official)  
- ClearTax Calculator  
- Economic Times Calculator

---

## 📧 Support & Contact

| Issue type | Where |
|---|---|
| Tax law questions | Income Tax Helpline |
| Technical problems | GitHub Issues |
| Feature requests | GitHub Discussions |
| Security concerns | security@example.com |
| General queries | support@example.com |

### Troubleshooting

<details>
<summary><b>Calculator not loading?</b></summary>

- Ensure JavaScript is enabled  
- Try incognito/private mode  
- Clear cache (Ctrl/Cmd + Shift + Delete)  
- Update browser to latest  
- Check console (F12)  
- Disable extensions temporarily  
- Try a different browser

</details>

<details>
<summary><b>Charts not displaying?</b></summary>

- Check internet (Chart.js CDN)  
- Disable ad/script blockers  
- Ensure `cdnjs.cloudflare.com` isn’t blocked  
- Wait for full page load  
- Verify Canvas support

</details>

<details>
<summary><b>Auto‑save not working?</b></summary>

- Enable LocalStorage  
- Check available space  
- Avoid private/incognito mode  
- Clear saved data: open console → `localStorage.clear()`  
- Try a different browser

</details>

<details>
<summary><b>Calculation seems off?</b></summary>

- Re‑check inputs & checkboxes  
- Compare with official calculator  
- Review breakdown tables  
- Confirm chosen regime  
- Open an issue with exact details

</details>

---

## 📜 License (MIT)

```
Copyright (c) 2025 India Tax Calculator Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

**What this means**  
✅ Free for personal & commercial use • ✅ Free to modify & distribute • ✅ No warranty • ✅ Keep license notice

---

<div align="center">

If this helped you, please ⭐ the repo!  
**Last Updated:** October 2025 • **Version:** 1.0.0

</div>
