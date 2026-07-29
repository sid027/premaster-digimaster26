# DigiMaster Pre-Master Days 2026 🎓

Welcome! This repository contains the self-study material for the DigiMaster Pre-Master Days 2026.

It teaches the four essential tools of the software world — **assuming zero prior technical knowledge**. Everything is explained step by step, in plain language, for **macOS** (Intel & Apple Silicon), **Windows** (10/11), and **Linux**.

One deliberate design choice: **everyone learns the same Linux commands.** Windows students install **WSL** (a real Linux inside Windows, an official Microsoft feature) in Notebook 1 — because the servers you will work with later in the program (Google Cloud) run Linux, and one command language learned once beats two learned badly.

## ⏳ Why this matters, and by when

**These skills are required to successfully finish the course.** They are not optional extras or background reading: the tools in these notebooks are the ones you will actually work with in class, and the course assumes you can use them.

That said — **you do not need to finish all the notebooks before the semester begins.** Nobody expects you to arrive on day one having completed everything. Start when you can and work at a pace that suits you.

Three things to keep in mind:

- **Follow the order: 01 → 02 → 03 → 04.** Each notebook builds on the one before it. Jumping ahead makes the later notebooks much harder than they need to be.
- **⚠️ Be through all four by the end of September / early October.** You will need these skills to successfully complete **Assignment 1**. Leaving them until the assignment is due means learning the tools and the assignment at the same time — which is a genuinely unpleasant way to spend a week.
- **Budget roughly 4–5 hours in total**, ideally split across a few sessions rather than one long evening. It sinks in better that way.

## 📚 The material — work through it in order

| # | File | What you learn | Time |
|---|---|---|---|
| 1 | [01-command-line.html](01-command-line.html) | Open a terminal (🪟 Windows: install Linux/WSL first) and talk to your computer in text: navigate, create, copy, delete — then install **Python 3.14 + Jupyter** as your graduation project | ~60–90 min |
| 2 | [02-git.ipynb](02-git.ipynb) | Track versions of your work with Git, undo mistakes, and sync with GitHub | ~60–90 min |
| 3 | [03-ssh.ipynb](03-ssh.ipynb) | Create your SSH key, log into remote servers, connect your key to GitHub | ~45–60 min |
| 4 | [04-docker.ipynb](04-docker.ipynb) | Run, build, and orchestrate software containers with Docker & Docker Compose | ~60–90 min |

> **Why is the first one a web page and the rest notebooks?** Because on day one you have nothing installed. Notebook 1 is a plain **web page** (`.html`) that opens in any browser — no tools, no accounts, nothing to set up. At the end of it you install **Jupyter**, and Jupyter is exactly what opens the other three, which are real **notebook files** (`.ipynb`). The course teaches you the tool you need to read the rest of the course.

Each notebook is **self-contained**: it includes the installation instructions for its own tool, checkpoints so you know you are on track, a troubleshooting section, and a cheat sheet.

## 🔑 How to read the material

### Notebook 1 — the web page 🌐

You have two ways to get it; both are fine.

**Easiest — download everything as a ZIP:**

1. On the repository page (<https://github.com/sid027/premaster-digimaster26>), click the green **`<> Code`** button.
2. Choose **Download ZIP**, then unzip the downloaded file (double-click it).
3. In the resulting folder, **double-click `01-command-line.html`** — it opens in your web browser, fully formatted. Start reading.

This also gets you the other notebooks and the example projects you need in Notebook 4, so it is the option we recommend.

**Or download just the one file:**

1. In the file list on GitHub, click **`01-command-line.html`**.
2. GitHub will show you the page's underlying code — that is expected, and not what you want to read. Click the **download icon** (⤓, top right of the file view) to save the file.
3. Double-click the downloaded file to open it in your browser.

> 💡 **Tip** — Keep two windows side by side: the notebook in your browser on one half of the screen, your terminal on the other half. You read on the left, you type on the right.

### Notebooks 2, 3 and 4 — the Jupyter notebooks 📓

**Read them in your browser (no setup):** click the file on GitHub — for example [02-git.ipynb](02-git.ipynb) — and it is displayed as a nicely formatted document. Nothing to install, works on any computer.

**Or open them in your own Jupyter (the real thing):** at the end of Notebook 1 you installed Jupyter, so you can read them the way they were written. In your terminal, go to the folder containing the files, activate the environment, and start Jupyter:

```
source .venv/bin/activate
```

```
jupyter lab
```

Then click a notebook in the file list on the left. (Notebook 1 walks through this in detail — it is the "daily ritual" at the end of section 9.)

> 💡 Double-clicking an `.ipynb` file on your computer without Jupyter shows unreadable raw text. That is normal — notebooks need a viewer, which is precisely why Notebook 1 has you install one.

### Keeping up to date with Git 🌳

From Notebook 2 onwards you can fetch the whole repository with a single command — the professional way, and exactly what you learn there:

```
git clone https://github.com/sid027/premaster-digimaster26.git
```

When your instructors update the material during the course, you get the newest version by running this inside the folder — no re-downloading:

```
git pull
```

## 🗺️ How to use this material

- **Just read the notebooks** — you never execute anything *inside* them. All commands are typed into the terminal **on your own computer** (Notebook 1 shows you how).
- Type the commands yourself instead of copy-pasting — that is how the vocabulary sticks.
- Don't skip the ✅ **Checkpoints** — they tell you whether you are on track before you move on.
- **Stuck?** Every notebook has a troubleshooting section near the end covering the errors beginners actually hit. Check there before assuming you broke something.

## 📁 What else is in this repository

| Folder | Used in | What it is |
|---|---|---|
| [`demo-app/`](demo-app/) | Notebook 4 | A tiny web application (Flask) that you package into a Docker image yourself — Dockerfile, app code, and a `compose.yaml` |
| [`database-demo/`](database-demo/) | Notebook 4 | A two-container system (PostgreSQL + Adminer) started with a single `docker compose up` — no code required |

---

*DigiMaster Pre-Master Days 2026 — have fun, and welcome to the technical side!* 🚀
