# GitHub Pages resume site

This repo contains a simple static site template for your resume, bio, LinkedIn link, and certifications.

## How to customize

### 1. Edit `index.html`:
- Replace the short bio and longer 'About' text.
- Replace the placeholder LinkedIn URL with your LinkedIn profile URL.

### 2. Add your resume:
- Upload a PDF named `assets/resume.pdf`.

### 3. Add certifications:

**Option A: Upload Certificate Images/PDFs**
1. Save your certificate files to the `certifications/` folder
   - Supported formats: PNG, JPG, PDF, SVG
   - Use descriptive names: `google-ai-essentials.png`, `aws-certification.pdf`
2. Edit `index.html` and add a new certification card in the certifications section:
```html
<div class="cert-card">
  <img src="certifications/your-cert.png" alt="Cert Name" class="cert-image">
  <div class="cert-info">
    <h3>Certification Name</h3>
    <p class="cert-issuer">Issuing Organization</p>
    <p class="cert-date">Month Year</p>
    <a href="verification-url" class="cert-link" target="_blank">View Certificate →</a>
  </div>
</div>
```

**Option B: Link to External Certifications**
If your certification is hosted elsewhere (Credly, LinkedIn, etc.), you don't need to upload files:
```html
<div class="cert-card">
  <div class="cert-info">
    <h3>Certification Name</h3>
    <p class="cert-issuer">Issuing Organization</p>
    <p class="cert-date">Month Year</p>
    <a href="https://external-link.com" class="cert-link" target="_blank">View Certificate →</a>
  </div>
</div>
```

See `certifications/README.md` for more detailed instructions and examples.

## Publishing (GitHub Pages)

- Go to your repo Settings → Pages and set the source to the `main` branch and the `/ (root)` folder. Save.
- Wait a minute; your site will be available at `https://<owner>.github.io/<repo>`.

If you want the site at `https://yourusername.github.io`, the repository must be named exactly `yourusername.github.io`.

## Quick Start for Adding Certifications

1. **Upload files**: Place certificate images in `certifications/` folder
2. **Edit HTML**: Add cert cards in `index.html` (copy the template from the file)
3. **Commit & Push**: Your changes will appear on GitHub Pages automatically
4. **Verify**: Visit your site to see the new certifications

## File Structure
```
.
├── index.html              # Main website file
├── assets/
│   ├── style.css          # Styling
│   └── resume.pdf         # Your resume (upload here)
├── certifications/         # Your certificate files
│   ├── README.md          # Detailed instructions
│   └── [your-certs.*]     # Upload certificates here
└── README.md              # This file
```