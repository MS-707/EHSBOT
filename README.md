# Mytra.ai SDS Portal

A mobile-friendly web portal for quick access to Safety Data Sheets.

## Features

- 🚨 **Emergency banner** with one-tap calling to 911 and CHEMTREC
- 🔍 **Search functionality** to quickly find chemicals
- ⚠️ **Prop 65 section** highlighting chemicals requiring warnings
- 📱 **Mobile-optimized** for scanning QR codes on the floor
- 🔗 **Direct SDS links** to manufacturer websites

## Deployment to Vercel

### Option 1: Deploy via Vercel CLI

1. Install Vercel CLI:
   ```bash
   npm install -g vercel
   ```

2. Navigate to this folder:
   ```bash
   cd SDS_Web_App
   ```

3. Deploy:
   ```bash
   vercel
   ```

4. Follow the prompts. Choose:
   - Set up and deploy: **Y**
   - Scope: Your account
   - Link to existing project: **N**
   - Project name: `mytra-sds` (or your choice)
   - Directory: `./`

5. Note your deployment URL (e.g., `https://mytra-sds.vercel.app`)

### Option 2: Deploy via GitHub + Vercel Dashboard

1. Push this folder to a GitHub repository

2. Go to [vercel.com](https://vercel.com) and sign in

3. Click "New Project"

4. Import your GitHub repository

5. Deploy (no configuration needed)

## After Deployment

1. **Update the QR code** with your actual URL:
   - The current QR code points to `https://mytra-sds.vercel.app`
   - If your URL is different, regenerate the QR code at [qr-code-generator.com](https://www.qr-code-generator.com/)

2. **Print the poster** (`SDS_QR_POSTER.png`) and laminate it

3. **Post near chemical storage areas**:
   - Near the flammable cabinet
   - At workstations where chemicals are used
   - In the receiving area

## Customization

### To add more chemicals:

Edit `index.html` and add entries in the appropriate category section:

```html
<div class="chemical-item" data-search="search keywords here">
    <div class="chemical-info">
        <div class="chemical-name">Product Name</div>
        <div class="chemical-mfr">Manufacturer</div>
    </div>
    <span class="badge badge-danger">DANGER</span>
    <a href="https://manufacturer-sds-url.com" target="_blank" class="sds-link">Get SDS →</a>
</div>
```

### To update emergency contacts:

Find the `emergency-section` in `index.html` and update the phone numbers.

### To add internal contacts:

Add a new `contact-card` div in the contact grid with your facility-specific numbers.

## Files Included

| File | Purpose |
|------|---------|
| `index.html` | Main web application (single-file, no dependencies) |
| `vercel.json` | Vercel deployment configuration |
| `qr_code.png` | QR code image (blue, high contrast) |
| `SDS_QR_POSTER.png` | Printable 8.5x11" poster with QR code |
| `README.md` | This file |

## Compliance Notes

This portal supplements (does not replace) the physical SDS binder required by:
- Cal/OSHA Title 8 CCR §5194
- OSHA 29 CFR 1910.1200

Per regulations, employees must have access to SDSs "without barriers." This digital portal provides an additional access method but a physical binder should remain available.

---

*Created: January 2025*
