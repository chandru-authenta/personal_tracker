# Second Brain

My personal dashboard for:

- **Learning**: concepts in my own words, each with a short "at a glance" summary, the notes, a confidence score and the links where I learned it.
- **Work log**: daily updates grouped by project, with status (in progress / blocked / done) and the next step.
- **Ideas & projects**: a board (Spark → Exploring → Building → Paused → Shipped) with what the AI thought about each idea.
- **Sources & chats**: every article, video and AI chat (Claude, ChatGPT, Gemini, Perplexity, Copilot…) in one searchable list, so I can find *where* I talked about something.
- **Dashboard**: quick capture, stats, a review queue, and a **"Pick these back up"** list of ideas and concepts I haven't touched in a while.

It's one HTML file with no build step, no server and no account.

## Host it on GitHub Pages

1. Create a new repository on GitHub (e.g. `second-brain`).
2. Upload `index.html` (and this README) to the repo: **Add file → Upload files → Commit**.
3. Open **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute your site is live at `https://<your-username>.github.io/second-brain/`.

## Where your data lives

Everything you add is saved in **your browser's local storage** on that device. That makes it fast and private, but:

- Clearing browser data erases it, so **back up regularly**: Settings → **Download data.json**. The dashboard reminds you every 7 days.
- To use it on another device, upload that `data.json` to the repo next to `index.html`. A browser that has no data yet loads it automatically, and any browser can pull it in with **Settings → Load data.json from site** (newer items win).
- ⚠️ On a free GitHub account, Pages repos are **public**, so anyone could open `your-site/data.json`. Keep private notes out of it, or move data between devices with **Import** instead of committing the file.

## Shortcuts

| Key | Action |
|---|---|
| `N` | New item (type depends on the page you're on) |
| `/` or `Ctrl/⌘ + K` | Search everything |
| `Ctrl/⌘ + Enter` | Save (in the editor or quick capture) |
| `Esc` | Close |

## Tips

- **Can't share an AI chat link?** In the link row, pick the AI from the dropdown (Claude, ChatGPT, Gemini…) and just describe it, like *"ChatGPT on phone, chat named 'SQL joins'"*. It still shows up under Sources & chats.
- Links are auto-detected: pasting a `claude.ai`, `chatgpt.com`, `gemini.google.com` or `perplexity.ai` link tags it as an AI chat.
- Notes support `**bold**`, `` `code` ``, `- bullet lists`, `# headings`, ``` code blocks ``` and plain URLs.
- Delete the example entries in Settings → **Remove examples**.
