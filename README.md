# Canton Fair Digital Business Card

## Setup Guide

### Step 1: Replace Placeholder Data

Edit `index.html` and `vcard.vcf` — search for these placeholders and replace with your real info:

| Placeholder | Replace With |
|-------------|-------------|
| `Saif YourLastName` | Your full name |
| `Your Company Name` | Your company name |
| `your_wechat_id` | Your actual WeChat ID |
| `+XXXXXXXXXXXX` | Your phone number with country code |
| `your.email@example.com` | Your email address |
| `yourwebsite.com` | Your website URL |
| `Your City, Your Country` | Your location |

### Step 2: Add Your WeChat QR Code

1. Open WeChat → Me → tap your name → "My QR Code"
2. Screenshot or save your QR code
3. Save it as `wechat-qr.png` in this folder (same directory as `index.html`)

### Step 3: Push to GitHub

```bash
# Create the repo on GitHub first, then:
cd canton-fair-card
git init
git add .
git commit -m "Digital business card for Canton Fair"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/canton-fair-card.git
git push -u origin main
```

### Step 4: Enable GitHub Pages

1. Go to your repo on GitHub
2. **Settings** → **Pages**
3. Source: **Deploy from a branch**
4. Branch: `main` → `/ (root)` → **Save**
5. Your card will be live at: `https://YOUR_USERNAME.github.io/canton-fair-card/`

### Step 5: Generate a QR Code for Your Card URL

Use any free QR code generator:
- https://www.qr-code-generator.com/
- https://qr.io/
- Or run locally: `npx qrcode-terminal "https://YOUR_USERNAME.github.io/canton-fair-card/"`

**Print this QR code on:**
- Your paper business cards
- A badge/lanyard holder insert
- A small printed card (visiting card size)
- Your phone's lock screen wallpaper

### Pro Tips for Canton Fair

1. **Save your card URL as an NFC tag** — tap phones to share
2. **Print the QR code large** — scanners in China expect visible QR codes
3. **Keep the page lightweight** — fair Wi-Fi can be spotty
4. **Also have a Chinese name card** (纸质名片) — some executives still prefer paper
5. **Test before you go** — scan the QR code yourself from another phone

### What People See When They Scan

1. Your digital business card loads in their phone browser
2. They see your info in English or Chinese (toggle)
3. They can copy your WeChat ID with one tap
4. They can download your VCF to save to contacts
5. They can scan your WeChat QR directly from the page

### File Structure

```
canton-fair-card/
├── index.html        # Digital business card (the main page)
├── vcard.vcf         # Downloadable contact file
├── wechat-qr.png     # Your WeChat QR (you add this)
└── README.md         # This file
```

### Privacy Note

Everything in this repo is **public**. Only include info you're comfortable sharing with anyone. Consider:
- Using a dedicated business phone number (not personal)
- Using a business email (not personal)
- Your WeChat ID is already semi-public by design
