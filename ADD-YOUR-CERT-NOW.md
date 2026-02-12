# 🎯 SIMPLE GUIDE: Add Your Certification Right Now

Hey Jackson! Here's exactly what you need to do to add your new certification using your LinkedIn post:

## What You See Now

Your website currently shows:
- **Card 1:** Google AI Essentials ✅ (already done)
- **Card 2:** Placeholder text that says "YOUR CERTIFICATION NAME" ⬅️ THIS IS WHERE YOU ADD YOURS!

## What To Do (3 Easy Steps)

### Step 1: Copy Your LinkedIn Post URL
1. Open your LinkedIn certification post in your browser
2. Copy the entire URL from the address bar
   - Example: `https://www.linkedin.com/posts/jackson-filosa_[text]-activity-[numbers]-[code]`

### Step 2: Edit the File
1. Open this file: `index.html`
2. Go to **line 54** (or search for "YOUR CERTIFICATION NAME")
3. You'll see this code:

```html
<!-- Certification 2 - REPLACE THIS WITH YOUR ACTUAL CERTIFICATION -->
<div class="cert-card">
  <div class="cert-info">
    <h3>YOUR CERTIFICATION NAME</h3>
    <p class="cert-issuer">Issuing Organization</p>
    <p class="cert-date">Month Year</p>
    <a href="YOUR_LINKEDIN_POST_URL_HERE" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

4. Replace these 4 things:
   - Line with `<h3>YOUR CERTIFICATION NAME</h3>` → Change to your cert name
   - Line with `<p class="cert-issuer">Issuing Organization</p>` → Change to who gave you the cert
   - Line with `<p class="cert-date">Month Year</p>` → Change to when you got it
   - Line with `href="YOUR_LINKEDIN_POST_URL_HERE"` → Paste your LinkedIn URL

### Step 3: Save and Push
```bash
git add index.html
git commit -m "Add my new certification"
git push
```

Done! Your website will update in 1-2 minutes.

## Real Example

If you got a "HubSpot Marketing" certification in February 2026, you'd change it to:

```html
<!-- Certification 2 -->
<div class="cert-card">
  <div class="cert-info">
    <h3>HubSpot Marketing</h3>
    <p class="cert-issuer">HubSpot Academy</p>
    <p class="cert-date">February 2026</p>
    <a href="https://www.linkedin.com/posts/jackson-filosa_hubspot-marketing-activity-7423456789012345678-XyZz" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

## Visual Preview

Your certifications section will look like this (with your actual cert instead of placeholder):

![Preview](https://github.com/user-attachments/assets/c7a85920-de7d-483f-be13-c8c285c01da5)

Both cards appear side by side on desktop, and stack on mobile.

## Add More Later?

Just copy the entire `<div class="cert-card">...</div>` block and paste it again before the closing `</div>` tag. You can add unlimited certifications this way!

---

**Questions?** Check out:
- `HOW-TO-ADD-CERTIFICATION.md` - More detailed version
- `certifications/QUICKSTART.md` - Alternative guide
- Comments in `index.html` - Template examples

Good luck! 🚀
