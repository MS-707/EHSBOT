# SDS Portal 

A mobile-friendly web portal for quick access to Safety Data Sheets.

## Features

- 🔍 **Search functionality** to quickly find SDS sheets for all hazardous chemicals used at Mytra.
- 📱 **Mobile-optimized** for accessing chemical information via QR code, or just on the go!
- 🔗 **Direct SDS links** to manufacturer provided chemical information.'
- **Timestamped updates** to maintain revision tracking of all manufacturer provided SDS

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

## Compliance Notes

This portal supplements (does not replace) the physical SDS binder required by:
- Cal/OSHA Title 8 CCR §5194
- OSHA 29 CFR 1910.1200

Per regulations, employees must have access to SDSs "without barriers." This digital portal provides an additional access method but a physical binder should remain available.

---

*Created: January 2026*
