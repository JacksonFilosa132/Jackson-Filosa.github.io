# Visual Guide: Exactly What to Edit

## The Section You Need to Edit

Open `index.html` and find **lines 54-62**. Here's what you'll see:

```html
54.    <!-- Certification 2 - REPLACE THIS WITH YOUR ACTUAL CERTIFICATION -->
55.    <div class="cert-card">
56.      <div class="cert-info">
57.        <h3>YOUR CERTIFICATION NAME</h3>
58.        <p class="cert-issuer">Issuing Organization</p>
59.        <p class="cert-date">Month Year</p>
60.        <a href="YOUR_LINKEDIN_POST_URL_HERE" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
61.      </div>
62.    </div>
```

## What to Change (4 Edits)

### Edit 1: Line 57 - Certification Name
**Change from:**
```html
<h3>YOUR CERTIFICATION NAME</h3>
```

**Change to:** (example)
```html
<h3>HubSpot Inbound Marketing</h3>
```

### Edit 2: Line 58 - Issuing Organization
**Change from:**
```html
<p class="cert-issuer">Issuing Organization</p>
```

**Change to:** (example)
```html
<p class="cert-issuer">HubSpot Academy</p>
```

### Edit 3: Line 59 - Date
**Change from:**
```html
<p class="cert-date">Month Year</p>
```

**Change to:** (example)
```html
<p class="cert-date">February 2026</p>
```

### Edit 4: Line 60 - LinkedIn URL
**Change from:**
```html
<a href="YOUR_LINKEDIN_POST_URL_HERE" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
```

**Change to:** (example - use YOUR actual LinkedIn post URL)
```html
<a href="https://www.linkedin.com/posts/jackson-filosa_inbound-marketing-activity-1234567890123456-AbCd" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
```

## Complete Example (After Your Edits)

If you got a "Salesforce Administrator" certification, your completed code would look like:

```html
54.    <!-- Certification 2 - Salesforce Administrator -->
55.    <div class="cert-card">
56.      <div class="cert-info">
57.        <h3>Salesforce Administrator</h3>
58.        <p class="cert-issuer">Salesforce</p>
59.        <p class="cert-date">January 2026</p>
60.        <a href="https://www.linkedin.com/posts/jackson-filosa_salesforce-admin-activity-7423456789012345-XyZz" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
61.      </div>
62.    </div>
```

## Before and After Preview

### BEFORE (what you see now):
```
┌─────────────────────────────┐  ┌─────────────────────────────┐
│  Google AI Essentials       │  │  YOUR CERTIFICATION NAME    │
│  Google                     │  │  Issuing Organization       │
│  2025                       │  │  Month Year                 │
│  [View Certificate →]       │  │  [View Certificate →]       │
└─────────────────────────────┘  └─────────────────────────────┘
```

### AFTER (after you edit):
```
┌─────────────────────────────┐  ┌─────────────────────────────┐
│  Google AI Essentials       │  │  Salesforce Administrator   │
│  Google                     │  │  Salesforce                 │
│  2025                       │  │  January 2026               │
│  [View Certificate →]       │  │  [View Certificate →]       │
└─────────────────────────────┘  └─────────────────────────────┘
```

## Save and Deploy

After making your edits:

```bash
git add index.html
git commit -m "Add Salesforce Administrator certification"
git push
```

Wait 1-2 minutes, then visit your website to see both certifications!

---

**Tip:** Keep the same format as the Google AI Essentials certification (lines 45-52) for consistency.
