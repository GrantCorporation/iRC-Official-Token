# GitHub Repository Setup for iRC Token Metadata

## Overview
This guide walks you through setting up a GitHub repository to permanently host your token metadata and images. GitHub raw URLs provide reliable, permanent hosting for Solana token metadata.

---

## Step 1: Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Create a **PUBLIC** repository named: `irc-token`
3. Owner should be: `iRunCrypto` (or your organization)
4. Add a description: "Official iRC Token metadata and assets"
5. Initialize with README: **Yes**
6. Click **Create repository**

---

## Step 2: Upload Assets

Upload these files to the repository:

### Required Files:
```
irc-token/
├── assets/
│   ├── irc-token-logo.png      (from: E:\iRC Official Token\assets\irc-token-logo.png)
│   └── irc-token-banner.png    (from: E:\iRC Official Token\assets\irc-token-banner.png)
├── metadata/
│   └── irc-token-metadata.json (from: E:\iRC Official Token\metadata\irc-token-metadata.json)
└── README.md
```

### Upload Methods:

**Option A: GitHub Web Interface**
1. Navigate to your repo
2. Click "Add file" → "Upload files"
3. Drag and drop the `assets` folder contents
4. Commit with message: "Add iRC token assets"
5. Repeat for `metadata` folder

**Option B: Git Command Line**
```bash
git clone https://github.com/iRunCrypto/irc-token.git
cd irc-token
mkdir assets metadata
cp "E:\iRC Official Token\assets\*" assets/
cp "E:\iRC Official Token\metadata\*" metadata/
git add .
git commit -m "Add iRC token metadata and assets"
git push origin main
```

---

## Step 3: Verify Raw URLs

After uploading, verify these URLs work (replace `iRunCrypto` with your actual GitHub username/org):

| Asset | Raw URL |
|-------|---------|
| **Logo** | `https://raw.githubusercontent.com/iRunCrypto/irc-token/main/assets/irc-token-logo.png` |
| **Banner** | `https://raw.githubusercontent.com/iRunCrypto/irc-token/main/assets/irc-token-banner.png` |
| **Metadata** | `https://raw.githubusercontent.com/iRunCrypto/irc-token/main/metadata/irc-token-metadata.json` |

Test each URL in your browser - you should see the image or JSON content directly.

---

## Step 4: Update Metadata JSON (if needed)

If your GitHub username is different from `iRunCrypto`, update the URLs in:
`E:\iRC Official Token\metadata\irc-token-metadata.json`

Replace all instances of:
```
https://raw.githubusercontent.com/iRunCrypto/irc-token/main/
```

With:
```
https://raw.githubusercontent.com/YOUR-USERNAME/irc-token/main/
```

---

## Final Metadata URLs

Once uploaded, your token will use:

```json
{
  "name": "iRC Token",
  "symbol": "iRC",
  "image": "https://raw.githubusercontent.com/iRunCrypto/irc-token/main/assets/irc-token-logo.png",
  "external_url": "https://iruncrypto.com/"
}
```

---

## Social Links in Metadata

Your token metadata includes these official links:

| Platform | URL |
|----------|-----|
| Website | https://iruncrypto.com/ |
| Twitter/X | https://x.com/iruncrypto |
| Discord | https://discord.gg/kSHgxSuF |
| Telegram | https://discord.gg/kSHgxSuF |

> ⚠️ **Note**: The Telegram link appears to be the same as Discord. Update if you have a separate Telegram link.

---

## Image Requirements

For best display across wallets and exchanges:

| Image | Recommended Size | Format |
|-------|-----------------|--------|
| Logo | 512x512 px (square) | PNG with transparency |
| Banner | 1200x630 px | PNG or JPG |

---

## Why GitHub Raw URLs?

✅ **Permanent** - URLs don't change as long as repo exists  
✅ **Free** - No hosting costs  
✅ **Fast** - GitHub CDN delivers globally  
✅ **Reliable** - 99.9% uptime  
✅ **Verifiable** - Anyone can audit the source  

---

## Next Steps

After setting up GitHub:
1. ✅ Verify all URLs are accessible
2. ✅ Proceed with token minting
3. ✅ Use metadata URL when uploading to Metaplex
