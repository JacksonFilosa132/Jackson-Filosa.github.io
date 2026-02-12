# Quick Start: Adding Certifications

## Step 1: Prepare Your Certificate Files
- Save your certificate images (PNG, JPG) or PDFs to the `certifications/` folder
- Use descriptive filenames: `google-cloud-cert.png`, `aws-certification.jpg`, etc.

## Step 2: Edit index.html
Open `index.html` and find the certifications section (around line 39).

### Option A: Add a Certificate with Image
Copy this template and paste it inside the `<div class="cert-grid">` section:

```html
<div class="cert-card">
  <img src="certifications/your-cert.png" alt="Certification Name" class="cert-image">
  <div class="cert-info">
    <h3>Certification Name</h3>
    <p class="cert-issuer">Issuing Organization</p>
    <p class="cert-date">Month Year</p>
    <a href="https://verify-link.com" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

### Option B: Link to External Certificate (No Upload Needed)
If your certificate is hosted online (Credly, LinkedIn, etc.):

```html
<div class="cert-card">
  <div class="cert-info">
    <h3>Certification Name</h3>
    <p class="cert-issuer">Issuing Organization</p>
    <p class="cert-date">Month Year</p>
    <a href="https://external-link.com" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate →</a>
  </div>
</div>
```

## Step 3: Commit and Push
```bash
git add .
git commit -m "Add new certification"
git push
```

Your changes will appear on your GitHub Pages site within a few minutes!

## Tips
- Keep image file sizes under 2MB for faster loading
- Always include verification links when available
- Use the same format for consistency across all certificates
- The cards are mobile-responsive and will stack on smaller screens
