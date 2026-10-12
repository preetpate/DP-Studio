# DP Studio

**Your Idea. Our Code. One Powerful Website.**

The official website of DP Studio, a small independent web studio that builds modern, responsive websites for businesses, creators and professionals. Websites start from ₹3,000+.

This is a single-page site made with plain HTML, CSS and JavaScript. There is no build step and no framework.

## Live projects

| Project | Type | Link |
|---|---|---|
| Prime Restaurant | Restaurant website | https://rastaurant-rfty.onrender.com/ |
| Prit Portfolio | Personal portfolio | https://preetpate.github.io/Prit-Portfolio/ |
| Chai & Co (sample) | E-commerce store with a working cart | https://preetpate.github.io/Shop/ |
| Sharma & Rao (sample) | Business website | https://preetpate.github.io/Business/ |
| Focusly (sample) | Landing page | https://preetpate.github.io/Landing-Page/ |
| Stockroom (sample) | Custom web app with login | https://preetpate.github.io/Custom/ |
| Pre-Agent AI v1.0 | AI-powered assistant | https://pre-agent.onrender.com/ |

Chai & Co, Sharma & Rao, Focusly and Stockroom are sample projects with fictional brands. They show what DP Studio can build.

## What is on the site

- **Navbar:** transparent at the top, blurred glass after scrolling. Links to every section and a "Let's Talk" button.
- **Hero:** headline, starting price, and two buttons ("Start a Project" and "Explore Our Work").
- **Trust strip:** a scrolling row of what every project includes.
- **Services:** six cards (Business Website, Landing Page, Portfolio, Restaurant, E-Commerce, Custom). Each card opens a live demo.
- **Our Work:** six real projects with links.
- **Pre-Agent:** a section for DP Studio's own AI assistant product.
- **Pricing:** Starter ₹3,000+, Business ₹5,000+, Custom ₹7,000+. Each button opens the inquiry form with the plan selected.
- **Documentation:** the project report that comes with every website.
- **Process:** five steps from idea to delivery.
- **Why DP Studio:** six reasons to choose the studio.
- **Help Me Choose:** opens the inquiry form for visitors who are not sure what they need.
- **Final call to action** and **footer**.
- **Inquiry form:** a pop-up form that sends an email (see below).
- **WhatsApp button:** floating button on desktop, sticky bottom bar on mobile.

## Files

```
index.html             the whole website (HTML, CSS and JavaScript)
README.md              this file
favicon.svg            browser tab icon (sharp at any size)
favicon-32.png         browser tab icon fallback
apple-touch-icon.png   icon used when the site is saved to a phone home screen
icon-512.png           large icon for social profiles and app listings
logo-mark.svg          the DP logo mark on its own
logo-wordmark.svg      logo mark with the "DP. STUDIO" wordmark
```

Upload every file in this folder to the repository root so the favicon and icons load.

## Settings you must change

Open `index.html` and search for `Settings`. You will find two values in the script near the bottom of the file.

### 1. WhatsApp number

```js
var WA_NUMBER = "";
```

Put your number in international format, digits only, with no `+` or spaces. Example for an Indian number: `"919876543210"`.

If you leave it empty, every WhatsApp button is hidden automatically, so no visitor ever lands on a broken link.

### 2. Email for the inquiry form

```js
var ACCESS_KEY = "PASTE_YOUR_WEB3FORMS_KEY";
```

1. Go to https://web3forms.com and enter the email address where you want to receive inquiries.
2. They send you a free access key by email.
3. Replace `PASTE_YOUR_WEB3FORMS_KEY` with that key.

Every inquiry then arrives in your inbox with the name, email, WhatsApp number, service, budget and project details. To send inquiries to both you and your partner, add the second address as a forwarding rule in your mail account.

If the key is not set, or sending fails, the form shows a ready summary with a **Copy inquiry** button (and a WhatsApp button if a number is set). The visitor never loses their message.

> Email only works when the site is hosted online (GitHub Pages, Render and so on). It does not work when you open `index.html` straight from your computer, or inside a private preview.

## Put it online with GitHub Pages

1. Create a new repository on GitHub, for example `DP-Studio`.
2. Upload all the files from this folder to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then click **Save**.
5. After a minute your site is live at `https://YOUR-USERNAME.github.io/DP-Studio/`.

To use your own domain, add it under **Settings → Pages → Custom domain**.

## How to edit

| To change | Search for |
|---|---|
| Prices | `₹3,000`, `₹5,000`, `₹7,000` |
| A project link | the project name, then edit its `href` |
| Colors | the `:root` block at the top of the `<style>` section |
| Studio name and tagline | `DP Studio` and `One Powerful Website` |
| Footer text | `Built by Dev & Preet` |

The colors are CSS variables: `--bg` (background), `--surface` (cards), `--a1` and `--a2` (the purple to blue accent), and `--muted` (secondary text).

## Logo

The mark is a **D** with a **P** cut into it, set on a purple-to-blue tile. It stays readable down to 16 pixels, so the same shape is used for the favicon. The wordmark is a heavy "DP." with "STUDIO" in small spaced capitals underneath.

## Design

- Dark premium style. Background `#080808`, cards `#111111`, accent gradient `#7C3AED` to `#2563EB`.
- Font: Manrope, with JetBrains Mono for small labels.
- Mobile first. Cards stack to one column, and a sticky bottom bar gives one-tap access to the inquiry form.
- Animations are light: text fade-in, card lift on hover, a slow floating browser window. They switch off for visitors who prefer reduced motion.

## Checklist before sharing the link

- [ ] `WA_NUMBER` is set
- [ ] `ACCESS_KEY` is set and a test inquiry reached your inbox
- [ ] Every project link opens
- [ ] Footer credits are correct

## Credits

Built by Dev & Preet at DP Studio.
