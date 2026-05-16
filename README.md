# AI Email Summarizer — Outlook Add-in

Summarize any email instantly using 1min.ai. Works on Outlook web, desktop, and mobile.

---

## What you need
- A free GitHub account (github.com)
- Your 1min.ai API key

---

## Setup: 5 steps

### Step 1 — Create a GitHub repository

1. Go to github.com and sign in
2. Click the **+** icon → **New repository**
3. Name it exactly: `outlook-summarizer`
4. Check **Public**
5. Click **Create repository**

---

### Step 2 — Upload the files

Upload these 3 files to your new repository:
- `taskpane.html`
- `manifest.xml`
- `commands.html`

To upload: click **Add file** → **Upload files** → drag all 3 files in → click **Commit changes**

---

### Step 3 — Enable GitHub Pages

1. In your repository, click **Settings**
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Set branch to **main**, folder to **/ (root)**
5. Click **Save**
6. Wait 1-2 minutes — your site will be live at:
   `https://YOUR-USERNAME.github.io/outlook-summarizer/`

---

### Step 4 — Update the manifest with your username

1. Open `manifest.xml` in GitHub (click the file, then the pencil ✏️ icon)
2. Use Find & Replace: replace every instance of `YOUR-GITHUB-USERNAME` with your actual GitHub username
3. Click **Commit changes**

---

### Step 5 — Install the add-in in Outlook

#### On Outlook Web (outlook.com) — also gives you mobile:
1. Open any email at outlook.com
2. Click the **three dots (...)** menu at the top of the email
3. Click **Get Add-ins**
4. Click **My add-ins** in the left panel
5. Scroll down to **Custom add-ins** → click **+ Add a custom add-in** → **Add from URL**
6. Paste this URL: `https://YOUR-USERNAME.github.io/outlook-summarizer/manifest.xml`
7. Click **OK** and confirm

#### On Outlook Desktop (Windows/Mac):
1. Open Outlook → click **Get Add-ins** in the ribbon
2. Follow the same steps as above from step 4

---

## Using the add-in

1. Open any email in Outlook
2. Click **AI Summarize** in the toolbar (desktop) or the **...** menu (mobile)
3. A sidebar opens — paste your 1min.ai API key the first time (it saves automatically)
4. Choose your preferred AI model
5. Click **Summarize this email** — done!

---

## Mobile (iOS / Android)

Once installed via outlook.com, the add-in automatically appears in the Outlook mobile app:
1. Open an email
2. Tap the **three dots (...)** at the bottom
3. Tap **AI Summarize**
4. The summary panel opens in-app

---

## Troubleshooting

**"Failed to fetch" error** — 1min.ai may have CORS restrictions for some origins. If this happens, let me know and we can add a simple proxy workaround.

**Add-in not showing on mobile** — make sure you installed it from outlook.com (web), not from the desktop app. Mobile sync comes from the web installation.

**Icon errors** — the add-in will still work even if icon images are missing. You can add an `icon.png` file to your repository later.
