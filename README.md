# Atharva Barkale — Portfolio

A single-page portfolio site (HTML + Tailwind CDN, no build step) with sections for
Home, About, Experience, Skills, Education, Projects, Certificates, and Contact.

## Files

- `index.html` — the whole site
- `profile.jpg` — your headshot, used in the hero card
- `Atharva_Prakash_Barkale_Resume.pdf` — linked from the "Download Resume" button
- `certificates/` — put your certificate images here (see below)

## 1. Add your certificate photos

Open the **Certificates** section in `index.html` and look for the two
placeholder cards (Cyber Security, Cloud Computing). Each one references:

```
certificates/cyber-security-cert.jpg
certificates/cloud-computing-cert.jpg
```

Drop your actual certificate photos into the `certificates/` folder using
those exact filenames (or update the `src`/`href` in `index.html` if you'd
rather name them differently). Until you add the images, each card shows a
placeholder icon instead of a broken image.

Add more cards by copying one of the existing `<div class="glass hover-card ...">`
blocks in the Certificates section.

## 2. Add real project links

In the **Projects** section, each card has GitHub / Live Demo links. Replace:

- `https://github.com/barkaleatharva4-sys/smart-hotel-ordering-system`
- `https://github.com/barkaleatharva4-sys/food-ordering-chatbot`
- `https://github.com/barkaleatharva4-sys/college-attendance-system`

with your actual repo URLs (create the repos on
https://github.com/barkaleatharva4-sys if they don't exist yet), and replace
the `href="#"` Live Demo placeholders with real deployed URLs once you have
them (e.g. after deploying each project to Vercel).

## 3. Push to GitHub

```bash
cd portfolio
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/barkaleatharva4-sys/portfolio.git
git push -u origin main
```

(Create the empty `portfolio` repo first at github.com/new under your
barkaleatharva4-sys account, then run the commands above.)

## 4. Deploy on Vercel

1. Go to https://vercel.com/barkaleatharva4-sys-projects
2. Click **Add New → Project**
3. Import the `portfolio` GitHub repo you just pushed
4. Framework preset: **Other** (it's plain HTML, no build command needed)
5. Click **Deploy**

Vercel will give you a live URL like `portfolio-yourname.vercel.app`. Every
time you push to `main` on GitHub, Vercel redeploys automatically.

## 5. Update the resume date range

The Education section flags that "Aug 2022 – Jul 2026" for your Diploma is
unusually long for a standard diploma program — double check this is correct
before publishing (it's currently taken as-is from your resume PDF).
