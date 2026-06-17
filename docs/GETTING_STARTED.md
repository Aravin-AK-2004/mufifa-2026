# Getting Started: Complete Beginner Guide

> **You don't need to know Git, the terminal, or any coding to participate in μFIFA.**
> This guide walks you through everything using only your web browser and GitHub's website.

---

## Before You Begin

You'll need:
- A laptop or desktop computer (phone works but is harder)
- An internet connection
- 20–30 minutes for your first setup

That's it. No installations required.

---

## Part 1: Create a GitHub Account

GitHub is a website where developers store and share code. We use it to host all μFIFA profiles.

1. Go to [github.com](https://github.com)
2. Click **Sign up** in the top right
3. Enter your email, create a password, and choose a username
4. Verify your email address
5. You're in ✅

> **Tip:** Choose a professional username. It will appear in your profile URL.

---

## Part 2: What is Markdown?

Markdown is a simple way to format text using plain characters. GitHub automatically renders it as styled text.

Here are the basics you need for your profile:

| What you type | What it looks like |
|---------------|-------------------|
| `# Big Heading` | Big Heading (H1) |
| `## Section` | Section (H2) |
| `### Sub-section` | Sub-section (H3) |
| `#### Sub-sub-section` | Sub-sub-section (H4) |
| `**bold text**` | **bold text** |
| `*italic text*` | *italic text* |
| `- item` | • item (bullet point) |
| `[link text](https://url.com)` | Clickable link |
| `> blockquote` | Indented quote block |

You don't need to memorise all of this. The [TEMPLATE.md](../TEMPLATE.md) already has all the formatting done for you. Just replace the placeholder text with your own words.

---

## Part 3: Fork the Repository

"Forking" means making your own personal copy of the μFIFA repository on GitHub. You'll edit your copy and then send the changes back.

**Step 1:** Go to the μFIFA repository:
👉 [https://github.com/gtech-mulearn/mufifa-2026](https://github.com/gtech-mulearn/mufifa-2026)

**Step 2:** Click the **Fork** button in the top-right corner of the page.

```
┌─────────────────────────────────────────────────────────┐
│  gtech-mulearn / mufifa-2026          [Star] [Fork] [⋯] │
└─────────────────────────────────────────────────────────┘
```

**Step 3:** On the "Create a new fork" page, leave everything as default and click **Create fork**.

You now have your own copy at `https://github.com/YOUR-USERNAME/mufifa-2026` ✅

---

## Part 4: Create Your Profile File

You'll do this entirely in your browser. No terminal or Git needed.

**Step 1:** In your forked repository, click on the **`profile`** folder.

**Step 2:** Click **Add file → Create new file** (top right of the file list).

**Step 3:** In the filename box at the top, type your MUID followed by `@mulearn.md`:

```
yourname@mulearn.md
```

For example, if your MUID is `sachinrajm@mulearn`, the file should be named:
```
sachinrajm@mulearn.md
```

> ⚠️ **Important:** The filename must exactly match your MUID (the one you got from the μLearn Discord).

**Step 4:** Copy the entire contents of [TEMPLATE.md](../TEMPLATE.md) and paste it into the editor.

**Step 5:** Replace every piece of placeholder text with your own content. See [this example](../profile/sachinrajm@mulearn.md) for inspiration.

> **Tip:** Click the **Preview** tab at the top of the editor to see how your profile will look when rendered.

---

## Part 5: Fill Out Your Profile

Open [TEMPLATE.md](../TEMPLATE.md) in a separate tab. Here's a section-by-section guide:

### Header (Line 1–2)
```markdown
# Full Name (Your Role / What You Do)
### Squad Domain: Coder | FIFA Nation: Brazil
```
Replace `Full Name` with your actual name. Replace `Coder` with your domain (Coder / Maker / Designer / Strategist). Replace `Brazil` with the FIFA nation you're representing.

### About Me
Write at least 200 characters about yourself. Think of it as your player bio: who you are, what you build, and why you're here. The validator will reject profiles with fewer than 200 characters, so write a proper paragraph.

### ⚽ FIFA World Cup Corner
Answer each sub-section honestly. There are no wrong answers. Share your football opinions, memories, and predictions.

### 🏅 Portfolio Highlights
Fill in your real work. If you're just starting out, write about what you're planning to build during μFIFA. Every section has a "If you're just starting" prompt to help you.

### Profile Card (Last Section)
Leave this for after Step 6 below.

---

## Part 6: Add Your μLearn Profile Card

Your profile card shows your live karma rank on the μLearn leaderboard.

**Step 1:** Join the [μLearn Discord server](https://discord.com/channels/771670169691881483/1157030408874106991)

**Step 2:** In Discord, type the command `/get-embed-link` and send it.

**Step 3:** Copy the link it gives you. It will look like:
```
https://mulearn.org/embed/rank/yourname@mulearn
```

**Step 4:** In your profile file, find the `#### Profile Card:` section at the bottom and replace `yourname@mulearn` in the `src=` URL with your actual MUID:

```html
<img
    src="https://mulearn.org/embed/rank/yourname@mulearn"
    width="400px">
</img>
```

So if your MUID is `sachinrajm@mulearn`, it becomes:
```html
<img
    src="https://mulearn.org/embed/rank/sachinrajm@mulearn"
    width="400px">
</img>
```

---

## Part 7: Save and Open a Pull Request

### Save your file
After writing your profile, scroll down on the GitHub editor page. You'll see a **"Commit changes"** section.

1. In the commit message box, write something like: `Add profile: yourname@mulearn`
2. Leave **"Commit directly to the `main` branch"** selected
3. Click **Commit changes**

### Open a Pull Request
A Pull Request (PR) is how you send your profile to the official μFIFA repository for review.

**Step 1:** Go to your forked repository's main page (`github.com/YOUR-USERNAME/mufifa-2026`).

**Step 2:** You'll see a yellow banner saying something like:
```
This branch is 1 commit ahead of gtech-mulearn:main
```
Click **Contribute → Open pull request**.

**Step 3:** On the Pull Request page:
- The title should auto-fill. Update it to: `[YOUR-MUID] - μFIFA World Cup 2026`
- Fill in the PR checklist (tick all the boxes you've completed)
- Click **Create pull request**

That's it. Your profile is submitted! ✅

---

## Part 8: What Happens Next?

After you open a PR, GitHub automatically runs a validator that checks:

| Check | What it looks for |
|-------|------------------|
| ✅ Filename | Must be `yourname@mulearn.md` |
| ✅ Header | Must have Squad Domain and FIFA Nation |
| ✅ About Me | Minimum 200 characters |
| ✅ All sections | Must all be present and filled |
| ✅ Profile Card | Must use your actual MUID |

If something fails, GitHub will show a red ❌ on your PR. Click on **Details** to see exactly what needs fixing. Fix it in your fork, commit again, and the check re-runs automatically.

If everything passes ✅, a maintainer will review and merge your PR. Welcome to μFIFA! ⚽

---

## FAQ: Common Questions and Errors

### "I don't know my MUID"
Watch the [Onboarding Video](https://www.youtube.com/watch?v=IwpOmzSqYao). It shows you exactly how to get your MUID from the μLearn Discord.

### "My file failed because the filename is wrong"
The file must be named exactly `yourname@mulearn.md` using your MUID. For example: `janedoe@mulearn.md`. No spaces, no capital letters in the MUID part.

### "About Me is too short"
Write more! 200 characters is roughly 2–3 sentences. The validator counts every character including spaces.

### "Profile Card still has the placeholder URL"
In the Profile Card section, make sure you replaced `yourname@mulearn` in the `src=` attribute with your actual MUID. The URL should look like `https://mulearn.org/embed/rank/janedoe@mulearn`.

### "I can't find the Fork button"
Make sure you're logged into GitHub first. The Fork button only appears when you're signed in.

### "The PR checklist is confusing"
Tick every box that applies to your profile. If a section is empty because you're just starting out, it's still okay. Write your plans instead of leaving it blank.

### "I made a mistake in my profile after submitting the PR"
Just edit the file in your fork again and commit the change. The PR will automatically update with the new version.

### "I'm stuck and nothing is working"
Ask for help in the `#μfifa-introduction` channel on the [μFIFA Discord server](https://discord.com/channels/771670169691881483/1157030408874106991). The community is here to help.

---

## 📚 Additional Resources

| Resource | Link |
|----------|------|
| Introduction to Markdown | [Discord guide](https://discord.com/channels/771670169691881483/1115381777792499805/1115727847647092808) |
| GitHub's "Hello World" guide | [docs.github.com/en/get-started](https://docs.github.com/en/get-started/quickstart/hello-world) |
| How to fork a repo (GitHub docs) | [docs.github.com: Fork a repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo) |
| How to open a Pull Request | [docs.github.com: PRs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) |
| μLearn Onboarding Video | [YouTube](https://www.youtube.com/watch?v=IwpOmzSqYao) |

---

<div align="center">

μFIFA World Cup 2026 · μLearn Foundation · You belong on this pitch.

</div>
