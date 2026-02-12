# Certifications Directory

This directory contains your certification files (images, PDFs, badges, etc.).

## How to Add Certifications

### Option 1: Add Certification Images
1. Save your certification image files (PNG, JPG, PDF) to this directory
2. Name them descriptively, e.g., `google-ai-essentials.png`, `aws-cloud-practitioner.pdf`
3. Update the `index.html` file in the certifications section to reference your files

### Option 2: Use External Links
- Link directly to online certifications (Credly badges, LinkedIn posts, etc.)
- These require no file upload, just update the HTML links

## Example Certification Entry

To display a certification with an image:

```html
<div class="cert-card">
  <img src="certifications/your-cert-image.png" alt="Certification Name" class="cert-image">
  <div class="cert-info">
    <h3>Certification Name</h3>
    <p class="cert-issuer">Issued by: Organization Name</p>
    <p class="cert-date">Date: Month Year</p>
    <a href="https://verify-link.com" class="cert-link" target="_blank">Verify Certificate</a>
  </div>
</div>
```

## Supported File Types
- Images: `.png`, `.jpg`, `.jpeg`, `.gif`, `.svg`
- Documents: `.pdf`

## Best Practices
- Use descriptive filenames (lowercase, hyphens instead of spaces)
- Keep file sizes reasonable (under 2MB per image)
- For PDFs, ensure they're optimized for web viewing
- Always include verification links when available
