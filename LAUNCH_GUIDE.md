# Verdant Global Services — Website Launch Guide

Your site is complete and ready to deploy. Follow these steps in order.

---

## Step 1 — Set up your Formspree email form

Before going live, wire up the contact form so quote requests reach your inbox.

1. Go to **https://formspree.io** and sign up for a free account (use Info@verdantglobalservices.com)
2. Click **New Form**, give it a name like "Verdant Quote Request"
3. Copy the form ID — it looks like `xpwzqrla`
4. Open `quote.html` in a text editor
5. Find this line near the top of the form:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
6. Replace `YOUR_FORM_ID` with your actual form ID, e.g.:
   ```
   action="https://formspree.io/f/xpwzqrla"
   ```
7. Save the file

Every quote submission will now be emailed to you automatically. The free plan covers 50 submissions/month. Upgrade if you expect more.

---

## Step 2 — Create a GitHub account (if you don't have one)

1. Go to **https://github.com** and sign up
2. Choose a username — something professional like `verdantglobalservices`
3. Verify your email address

---

## Step 3 — Create your repository

1. Once logged in, click the **+** icon (top right) → **New repository**
2. Repository name: `verdant-global-services` (or any name you prefer)
3. Set it to **Public** (required for free GitHub Pages hosting)
4. Do NOT check "Add a README file"
5. Click **Create repository**

---

## Step 4 — Upload your website files

You have two options:

### Option A — Upload via browser (easiest, no technical knowledge needed)

1. On your new repository page, click **uploading an existing file**
2. Drag and drop ALL the files and folders from your project folder:
   - `index.html`
   - `industries.html`
   - `sourcing.html`
   - `logistics.html`
   - `quote.html`
   - `about.html`
   - `css/` folder
   - `js/` folder
   - `brand/` folder
3. Scroll down, write a commit message like "Initial site upload"
4. Click **Commit changes**

> **Important:** The folder structure must be preserved. `css/styles.css`, `js/main.js`, and `brand/*.svg` must be in their folders, not at the root level.

### Option B — Via GitHub Desktop app (easier for future updates)

1. Download GitHub Desktop from **https://desktop.github.com**
2. Sign in with your GitHub account
3. Clone your new repository to your computer
4. Copy all your site files into the cloned folder
5. In GitHub Desktop, write a commit message and click **Commit to main**
6. Click **Push origin**

---

## Step 5 — Enable GitHub Pages

1. In your repository, click **Settings** (top tab row)
2. In the left sidebar, click **Pages**
3. Under "Source", select **Deploy from a branch**
4. Under "Branch", select **main** and **/ (root)**
5. Click **Save**
6. Wait 1–2 minutes, then refresh the page
7. GitHub will show you your live URL: `https://yourusername.github.io/verdant-global-services/`

Your site is now live.

---

## Step 6 — Connect a custom domain (recommended)

A custom domain like `verdantglobalservices.com` looks far more professional than a GitHub URL.

### Buy the domain

Go to any domain registrar — **Namecheap** (namecheap.com) or **Google Domains** (domains.google) are straightforward. Search for `verdantglobalservices.com` and purchase it (~$12–15/year).

### Point the domain to GitHub Pages

In your domain registrar's DNS settings, add these records:

| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | yourusername.github.io |

Then in GitHub Pages settings:
1. Under "Custom domain", type `verdantglobalservices.com`
2. Click **Save**
3. Check **Enforce HTTPS** (gives you the padlock/secure badge)

DNS changes take 15 minutes to 48 hours to propagate worldwide.

---

## Step 7 — Test your live site

Once live, check the following:

- [ ] All 6 pages load correctly (Home, Industries, Sourcing, Logistics, Quote, About)
- [ ] Logo appears in the navigation on every page
- [ ] Images load (offshore platform, excavator, combine harvester, etc.)
- [ ] "Request a Quote" form submits successfully — check your Formspree dashboard
- [ ] You receive a test email after submitting the form
- [ ] Phone number `+1 707-676-3876` is clickable on mobile
- [ ] Email `Info@verdantglobalservices.com` opens a mail client when clicked
- [ ] Site looks correct on a mobile phone (test by opening on your phone)

---

## Making future updates

Whenever you need to update text, add pages, or change images:

1. Edit the file(s) locally on your computer
2. Re-upload the changed file(s) to GitHub (replace the old version)
3. GitHub Pages republishes automatically within 1–2 minutes

---

## Need help?

- GitHub Pages documentation: https://docs.github.com/pages
- Formspree documentation: https://help.formspree.io
- For domain DNS help, contact your registrar's support chat

---

*Guide prepared for Verdant Global Services website — June 2026*
