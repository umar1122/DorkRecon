# Dorking For Bug Bounty — Recon

![License: MIT](https://img.shields.io/badge/license-MIT-3fb68a.svg)
![Type: Static site](https://img.shields.io/badge/type-static%20site-e8a33d.svg)
![Made with](https://img.shields.io/badge/made%20with-HTML%20%2B%20CSS%20%2B%20JS-e15a4d.svg)

**Live site:** replace this line with your GitHub Pages link once it's deployed, e.g. (https://umar1122.github.io/DorkRecon/)

A simple webpage that lists useful **Google, Shodan, and GitHub search tricks** (called "dorks") that security researchers use to find exposed files, weak logins, and leaked secrets — as part of legal bug bounty hunting.

It's just one HTML file. No installation, no server, no coding needed to use it.

---

## What is a "dork"?

A dork is just a smart search query. Instead of typing "cat pictures" into Google, you type something like:

```
filetype:env "DB_PASSWORD"
```

That tells Google: "find me `.env` files on the internet that contain the text `DB_PASSWORD`." Shodan and GitHub have their own versions of this trick, searching devices and code instead of web pages.

Bug bounty hunters use dorks as a starting point to find things a company forgot to lock down — like an exposed config file or an admin panel with no password.

---

## What this website does

- Shows a list of ready-to-use dorks, split into three tabs: **Google**, **Shodan**, and **GitHub**.
- Each dork has a short plain-English description of what it finds.
- You can type a **domain** (like `example.com`) at the top and click **Apply** — the site automatically fills that domain into every dork that needs it.
- Click **search** next to any dork to open it directly in Google, Shodan, or GitHub, with your domain already filled in.
- Click **copy** to copy a dork to your clipboard instead.
- Tick the **checkbox** next to a dork once you've tried it. The site remembers which ones you've used (saved only in your own browser — nothing is uploaded anywhere).
- Use the **search box** at the top to filter the list by keyword, like "mongodb" or "aws".

---

## How to use it, step by step

1. Open the website (see the hosting guide below if you haven't put it online yet).
2. Pick the target you're allowed to test — for example, a company running a public bug bounty program.
3. Type their domain into the **domain** box and click **Apply**.
4. Go through each tab (Google, Shodan, GitHub) and click **search** on the dorks that make sense for that target.
5. Check anything interesting you find against the bug bounty program's rules before reporting it.
6. Tick the checkbox on dorks you've already tried, so you don't repeat yourself next time.

---
---

## ⚠️ Important: use this responsibly

**This project is for research and education only.**

Only use these dorks on:
- Your own websites, servers, and accounts, **or**
- Public bug bounty programs (like HackerOne, Bugcrowd, Intigriti, or a company's own program) that have **explicitly given permission** to be tested, and only **within the scope and rules** that program sets.

Do **not** use these dorks against any website, company, or system you don't have permission to test. Searching for and accessing data you're not authorized to access is illegal in most countries, even if the data was easy to find. Finding something with a dork does not mean you're allowed to access, download, or use it — always follow the target program's disclosure rules and report responsibly.

The author of this project is not responsible for how it is used.

---

## License

This project is released under the MIT License — see the [LICENSE](LICENSE) file for the full text. In short: you're free to use, copy, modify, and share this project, including for commercial purposes, as long as you keep the original license notice.
