# How to Add Your Certification

## Quick Steps to Add a New Certification Using LinkedIn Post

You already have one certification (Google AI Essentials). Here's how to add another one:

### Step 1: Get Your LinkedIn Post URL
1. Go to your LinkedIn certification post
2. Copy the full URL from your browser
   - It should look like: `https://www.linkedin.com/posts/jackson-filosa_[hashtags]-activity-[numbers]-[code]`

### Step 2: Edit index.html
1. Open the `index.html` file
2. Find the certifications section (around line 43-67)
3. Copy the existing certification card code
4. Paste it right after the first one, but BEFORE the closing `</div>` tag

### Step 3: Update Your New Certification Details

**Here's the template to copy:**

```html
<div class="cert-card">
  <div class="cert-info">
    <h3>YOUR CERTIFICATION NAME HERE</h3>
    <p class="cert-issuer">ISSUING ORGANIZATION</p>
    <p class="cert-date">MONTH YEAR</p>
    <a href="YOUR_LINKEDIN_POST_URL_HERE" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

### Step 4: Replace the Placeholders

Replace these parts with your information:
- `YOUR CERTIFICATION NAME HERE` - e.g., "AWS Cloud Practitioner"
- `ISSUING ORGANIZATION` - e.g., "Amazon Web Services"
- `MONTH YEAR` - e.g., "February 2026"
- `YOUR_LINKEDIN_POST_URL_HERE` - Your full LinkedIn post URL

### Example:

If you earned a "Salesforce Administrator" certification in January 2026, your code would look like:

```html
<div class="cert-card">
  <div class="cert-info">
    <h3>Salesforce Administrator</h3>
    <p class="cert-issuer">Salesforce</p>
    <p class="cert-date">January 2026</p>
    <a href="https://www.linkedin.com/posts/jackson-filosa_salesforce-admin-certification-activity-1234567890123456-AbCD" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

### Step 5: Where Exactly to Add It

In your `index.html` file, locate this section:

```html
<div class="cert-grid">
  <!-- Example Certification Card with External Link -->
  <div class="cert-card">
    <div class="cert-info">
      <h3>Google AI Essentials</h3>
      <p class="cert-issuer">Google</p>
      <p class="cert-date">2025</p>
      <a href="https://www.linkedin.com/posts/jackson-filosa_googleai-artificialintelligence-aicertification-activity-7422016853323198464-JaSD" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
    </div>
  </div>
  
  <!-- ADD YOUR NEW CERTIFICATION HERE! -->
  
  <!-- Add more certifications here following the same pattern:
```

Insert your new certification card where it says "ADD YOUR NEW CERTIFICATION HERE!"

### Step 6: Save and Deploy

1. Save the `index.html` file
2. Commit your changes:
   ```bash
   git add index.html
   git commit -m "Add new certification"
   git push
   ```
3. Wait 1-2 minutes for GitHub Pages to update
4. Visit your website to see the new certification!

## Visual Result

Both certifications will appear as cards side by side on desktop, and stacked on mobile devices. They'll have:
- Hover effects (cards lift when you hover over them)
- Professional styling matching your site
- Direct links to your LinkedIn posts

## Need Help?

- See `certifications/README.md` for more detailed instructions
- See `certifications/QUICKSTART.md` for step-by-step guidance
- Check the comments in `index.html` for the template

---

**Pro Tip:** You can add as many certifications as you want by repeating this process!
