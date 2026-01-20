# SDS Portal Maintenance Cheat Sheet

## Quick Reference

| Task | Time | Difficulty |
|------|------|------------|
| Add a chemical | 2 min | Easy |
| Remove a chemical | 1 min | Easy |
| Update an SDS link | 30 sec | Easy |
| Update "Last Updated" date | 30 sec | Easy |

---

## Adding a New Chemical

### Step 1: Gather Info
- Product name
- Manufacturer
- CAS number (if applicable)
- SDS URL from manufacturer website

### Step 2: Add to index.html

Add the chemical in **TWO places**:

1. **Alphabetical Index (A-Z)** - around line 295, in alphabetical order
2. **Category section** - find the right category (Adhesives, Coatings, etc.)

**Copy this template:**
```html
<div class="chem" data-search="manufacturer product-name cas-number keywords">
    <div class="chem-info">
        <div class="chem-name">Product Name</div>
        <div class="chem-mfr">Manufacturer | CAS: XX-XX-X</div>
    </div>
    <a href="SDS_URL_HERE" target="_blank" class="sds-btn">View SDS</a>
</div>
```

**Tips for data-search:**
- Use lowercase
- Include manufacturer name, product name, CAS number
- Add common search terms (e.g., "grease lubricant" or "adhesive glue")

### Step 3: Update Counts
Find the category header and update the count number:
```html
<span class="count">74</span>  <!-- Change this number -->
```

### Step 4: Update "Last Updated" Date
Find this line near the top of the HTML (around line 265):
```html
<div class="last-updated">Last updated: January 19, 2026</div>
```
Change the date to today's date.

### Step 5: Deploy
```bash
cd "/Users/markstarrpro/Desktop/Mytra EHS Program Management/SDS/Photos/Mytra_Chemical_Inventory/SDS_Web_App"
git add index.html
git commit -m "Add [Chemical Name]"
git push
```

Vercel deploys automatically in ~30 seconds.

---

## Removing a Chemical

1. Delete the `<div class="chem">...</div>` block from **both** A-Z and category sections
2. Update the count numbers in category headers
3. Update the "Last Updated" date
4. Commit and push

---

## Updating an SDS Link

1. Open index.html
2. Cmd+F (or Ctrl+F) for the chemical name
3. Replace the URL in the `href="..."` attribute
4. Update the "Last Updated" date
5. Commit and push

---

## Categories Reference

| Category | CSS Class | Color |
|----------|-----------|-------|
| Alphabetical Index | cat-az | Purple |
| Adhesives & Sealants | cat-adhesives | Pink |
| Coatings & Paints | cat-coatings | Violet |
| Construction Materials | cat-construction | Stone |
| Cutting & Machining Fluids | cat-cutting | Amber |
| Electronics Materials | cat-electronics | Cyan |
| Fuels & Compressed Gas | cat-fuels | Red |
| Lubricants & Greases | cat-lubricants | Green |
| Prop 65 Chemicals | cat-prop65 | Warning Yellow |
| Solvents & Cleaners | cat-solvents | Blue |

---

## Verification Checklist

After any update:
- [ ] Visit https://ehsbot.vercel.app/
- [ ] Search for the chemical you added/changed
- [ ] Click "View SDS" to verify the link works
- [ ] Check that the count numbers are correct
- [ ] Verify "Last Updated" shows today's date

---

## Rollback (If Something Breaks)

```bash
# See recent commits
git log --oneline -5

# Undo the last commit
git revert HEAD
git push
```

---

## File Location

```
/Users/markstarrpro/Desktop/Mytra EHS Program Management/SDS/Photos/Mytra_Chemical_Inventory/SDS_Web_App/index.html
```

---

## Live Site

https://ehsbot.vercel.app/

---

## Support

GitHub Repo: https://github.com/MS-707/EHSBOT
