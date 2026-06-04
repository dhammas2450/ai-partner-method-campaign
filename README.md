# AI Partner Method - Affiliate Campaign

## Campaign Overview
**Product:** AI Partner Method by Philip Johansen
**Affiliate:** Donald Hammas (DVH Ventures LLC / DVH Nexus)
**Campaign Created:** June 4, 2025

---

## Campaign Assets

### 1. Sales Page
- **Location:** `sales-page/index.html`
- **Style:** Matches AI Partner Method branding (red/black gradient)
- **Content:** Hero, problem, solution, features, bonuses, CTAs
- **Affiliate Link:** https://www.aipartnermethod.com/success-with-donald-hammas

### 2. Bonus Delivery Page
- **Location:** `bonus-delivery/index.html`
- **Purpose:** Thank you page for buyers to access bonuses
- **Includes:** All 5 bonuses with download buttons, next steps, support info

### 3. Email Sequences
- **Pre-Sell Sequence:** `emails/presell-sequence.md` (3 emails)
- **Sales Sequence:** `emails/sales-sequence.md` (7 emails)

### 4. Strategy Documents
- **Hooks:** `hooks.md` - 7 angles for promotion
- **Pre-Sells:** `presells.md` - 3 pre-sell resource ideas
- **Bonuses:** `bonuses.md` - 5 bonus descriptions
- **Analysis:** `offer-analysis.md` - Product research

---

## Deployment Steps

### Step 1: Create GitHub Repository
```bash
cd ~/.openclaw/workspace/campaigns/ai-partner-method
git init
git add .
git commit -m "Initial campaign setup"
# Create repo on GitHub and push
```

### Step 2: Deploy to Vercel
1. Import GitHub repo to Vercel
2. Deploy sales-page folder → gets URL like `ai-partner-sales.vercel.app`
3. Deploy bonus-delivery folder → gets URL like `ai-partner-bonuses.vercel.app`

### Step 3: Create GlobalControl Tag
```bash
POST https://api.globalcontrol.io/api/ai/tags
{
  "name": "int-aipartnermethod",
  "description": "Interest in AI Partner Method",
  "groupId": "67368a8c3c07f60ff036f2b2"
}
```

### Step 4: Create GlobalControl Workflow
Create workflow with 7 email sequence triggered by `int-aipartnermethod` tag.

### Step 5: Create Letterman Publication
Set up publication for blog content/social distribution.

---

## File Structure
```
ai-partner-method/
├── README.md
├── offer-analysis.md
├── hooks.md
├── presells.md
├── bonuses.md
├── sales-page/
│   └── index.html
├── bonus-delivery/
│   └── index.html
└── emails/
    ├── presell-sequence.md
    └── sales-sequence.md
```

---

## Quick Stats
- **Hooks:** 7 angles
- **Pre-sells:** 3 planned
- **Bonuses:** 5 ($2,385 total value)
- **Emails:** 10 total (3 presell + 7 sales)
- **Campaign Value:** Complete affiliate system
