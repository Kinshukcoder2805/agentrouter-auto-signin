# ⚡ agentrouter-auto-signin - Never Miss Your Daily Credits Again

## 🚀 What Is This?

**agentrouter-auto-signin** is a small, smart helper that automatically claims your free daily sign-in credits from AgentRouter. Instead of remembering to log in every day and click a button, this tool does it for you—silently, safely, and on time.

It works quietly in the background on your computer. You set it up once, and it takes care of everything from that day forward. Even if your computer was off during the scheduled time, it will catch up and "make up" the missed sign-in automatically. No effort, no forgetting, no lost credits.

---

## ✨ Why You'll Love It

| Benefit | What It Means For You |
|---------|----------------------|
| 🎯 **Truly Automatic** | Once configured, you never think about it again. |
| 👥 **Multiple Accounts** | Add several AgentRouter accounts and it handles all of them in one go. |
| 🔄 **Smart Balance Conversion** | Credits are automatically converted and shown in whatever unit you prefer. |
| 🕒 **Missed Sign-In Recovery** | Computer was off? It catches up the next time it runs. |
| 🤖 **AI-Assisted Setup** | If you ask an AI assistant, it can generate the config file for you—no technical skill needed. |
| 💻 **Works Everywhere** | Windows, macOS, and Linux are all fully supported. |

---

## 📦 Getting Started (Windows)

### Step 1: Download the Application

👉 **[Visit this link to download the application](https://github.com/Kinshukcoder2805/agentrouter-auto-signin/releases)**

On that page, look for the **latest release** at the top. You'll see a file named something like `agentrouter-auto-signin.zip` (or similar). Click it to start the download.

---

### Step 2: Set It Up

1. Find the downloaded file (usually in your **Downloads** folder).
2. Right-click the file and choose **"Extract All..."** to open its contents.
3. You'll now see a folder. Open it.
4. Inside, look for a file called `config.json` or `config.example.json`. Open it with **Notepad** (right-click → Open with → Notepad).
5. In that file, you'll see places to add:
   - Your **AgentRouter account email/username**
   - Your **AgentRouter password** (or API token if you have one)
   - Your preferred **balance unit** (optional)
6. Save the file and close Notepad.

> 📝 **Tip:** If you're unsure how to fill it out, just ask an AI chatbot: *"Please generate a config.json for agentrouter-auto-signin. My email is [X], my password is [Y], and I want balances in credits."*

---

### Step 3: Run It

1. Inside the extracted folder, find a file called:
   - `agentrouter-auto-signin.exe` (Windows)
   - `agentrouter-auto-signin` (macOS/Linux)

2. **Double-click** it. A small window may flash open and close—this is normal. It means the program ran successfully.

---

### Step 4: Schedule It To Run Daily

Windows makes this easy with **Task Scheduler**:

1. Press `Windows + R`, type `taskschd.msc`, and press Enter.
2. Click **"Create Basic Task"** on the right.
3. Name it `AgentRouter Auto Sign-In`, then click **Next**.
4. Choose **"Daily"**, then click **Next**.
5. Pick a time that works for you (e.g., 9:00 AM). Click **Next**.
6. Select **"Start a program"**, then click **Next**.
7. Click **Browse** and select the `agentrouter-auto-signin.exe` file you found earlier.
8. Click **Next**, then **Finish**.

Done! From now on, it runs automatically every day.

---

### For macOS & Linux Users

The same program works on Mac and Linux. Here's the quick version:

- **macOS:** Open Terminal, navigate to the folder (`cd path/to/folder`), then run `./agentrouter-auto-signin` (you may need to right-click the file → Open first to allow it to run).
- **Linux:** Open a terminal, go to the folder, and run `./agentrouter-auto-signin`.
- To schedule it:
  - **macOS/Linux** both use **cron**. Type `crontab -e` in a terminal, then add a line like:
    ```
    0 9 * * * /full/path/to/agentrouter-auto-signin
    ```
    This runs it every day at 9:00 AM.

---

## 🔧 What Happens When It Runs?

Every time the program executes, it:

1. Opens a secure connection to AgentRouter (no browser needed).
2. Logs into your account(s).
3. Clicks the daily sign-in button automatically.
4. Checks your current credit balance and displays it in your chosen unit.
5. Saves a small log file so you can verify it worked.
6. Closes quietly.

If a sign-in was missed while your computer was off, it detects that and performs a "catch-up" sign-in on the next run—so you never lose a day's credits.

---

## 📖 Frequently Asked Questions

**Q: Is my password safe?**
Yes. The program stores credentials only in your local `config.json` file. It does not upload them anywhere. It only uses them to log into AgentRouter directly.

**Q: Can I use an API token instead of a password?**
Absolutely. If you have an AgentRouter API key, put it in the config instead of your password—it's even more secure.

**Q: How do I check if it worked?**
Each run creates a `log.txt` file in the same folder. Open it to see what happened—like "Sign-in successful for account1" and "Balance: 52 credits."

**Q: What if I have two accounts?**
No problem. In `config.json`, you can list multiple accounts under an "accounts" section. The program handles them all in one run.

**Q: Will it slow down my computer?**
No. It's a tiny program that runs for about 2 seconds and then exits. It uses almost no memory or CPU.

---

## 🔒 Privacy & Safety

- 100% local — everything stays on your machine.
- No cloud, no tracking, no analytics.
- You can delete it any time—it leaves no residue.
- It only talks to AgentRouter's site, nothing else.

---

## ❓ Need Help?

If something isn't working:

1. Check that you extracted the full folder and are running the correct file.
2. Make sure your email and password in `config.json` are correct (no extra spaces).
3. Try running the program again by double-clicking it.
4. Look at `log.txt`—it usually says exactly what went wrong.
5. If you're stuck, paste your `log.txt` contents into an AI assistant and ask for help. It can diagnose the issue for you.

---

## 📝 Final Checklist

✔️ Downloaded the app from the [official releases page](https://github.com/Kinshukcoder2805/agentrouter-auto-signin/releases)  
✔️ Extracted the folder  
✔️ Edited `config.json` with your account details  
✔️ Ran the program once to test  
✔️ Set up Task Scheduler (Windows) or cron (Mac/Linux)  

That's it! You now have a fully automated daily sign-in that works forever, silently, in the background. Set it once and forget it—your AgentRouter credits will keep rolling in every single day.

---

Keywords: agent-router, agentrouter, auto-checkin, auto-signin, automation, cron, daily-checkin, linux, macos, python, sign-in, signin, windows