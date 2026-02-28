# IRAH - GitHub

> [!tip]- Guide - Locating Obsidian Vault Folder and Syncing to GitHub
> Perfect. Targeting that specific folder is the smartest move because it captures the entire "Startup" ecosystem, not just the code.
> 
> ![[../z-Attachments/Terminal Copy Pathname.png|600]]
> 
> Since your folder name has spaces and an emoji, the Terminal can be a bit picky. Follow these exact steps to link your main Startup folder to your GitHub:
> 
> ### **Step 1: Navigate to the Startup Folder**
> 
> Open your Terminal and paste this exact command (the quotes are important because of the spaces):
> 
> ```bash
> cd "/Users/shieramaylaran/Obsidian Vault/Shiera 2.0/IRAH - Tech StartUp 💻"
> 
> ```
> 
> *To verify you are in the right place, type `ls`. You should see your folders and notes listed.*
> 
> ---
> 
> ### **Step 2: Initialize and Sync**
> 
> Run these commands one by one. This will take all your current notes and prepare them for your GitHub "IRAH-Coding-Basics-Journey" repository.
> 
> 1. **Initialize Git:**
> `git init`
> 2. **Add all files:**
> `git add .`
> 3. **Commit your progress:**
> `git commit -m "Initial sync of IRAH Startup Vault"`
> 4. **Connect to your GitHub:**
> `git remote add origin https://github.com/StyledByShiera/IRAH-Coding-Basics-Journey.git`
> 5. **Final Push:**
> `git push -u origin main -f`
> *(The `-f` forces the sync to ensure your local vault becomes the "master" version on GitHub.)*
> 
> ---
> 
> ### **Step 3: Set up Auto-Sync (The "Regional Director" Workflow)**
> 
> As a busy Director, you don't want to manually type these commands every time you finish a note. Here is how to make it automatic:
> 
> 6. **Install the "Obsidian Git" Plugin:** In Obsidian, go to `Settings` > `Community Plugins` > `Browse` > Search for **Obsidian Git**.
> 7. **Enable Auto-Backup:** In the plugin settings, look for **Vault backup interval (minutes)**. Set this to `30` or `60`.
> 8. **Auto-Pull:** Enable "Pull updates on startup" so if you ever edit your notes on another device, your laptop stays updated.
> 
> ---
> 
> ### **My "Grounded" AI Peer Advice:**
> 
> Shiera, because this is your "Shiera 2.0" folder, your GitHub contribution graph (those green squares) is about to explode with activity!
> 
> One thing to note: GitHub is public by default. If you have sensitive company info (like specific Trends & Concepts debt numbers or private BPO client names) in those notes, make sure your GitHub repository is set to **"Private"** in the GitHub Settings tab. You can still show your progress to others, but the specific contents will be shielded.
> 
> **Did the push command work? Once you see "Branch 'main' set up to track...", your entire Startup journey is officially backed up!**

###### M1 and GitHub Handshake Guide:
> [!info]- How to create a TOKEN in GitHub
> No worries at all, Shiera! This is a very common "Site Ocular" roadblock. GitHub actually **disabled normal passwords** for terminal actions back in 2021 for security reasons. Even if you remembered your password, it would still give you that error.
> 
> Since it's nearly midnight on February 28, let’s get this "Handshake" fixed so you can start March 1 with a win.
> 
> ### **The Fix: Generate a Personal Access Token (PAT)**
> 
> Think of this as a **Special Entry Permit** just for your laptop.
> 
> 1. **Go to GitHub.com** in your browser.
> 2. Click your profile photo (top right) > **Settings**.
> 3. Scroll all the way down on the left sidebar to **Developer settings**.
> 4. Click **Personal access tokens** > **Tokens (classic)**.
> 5. Click **Generate new token** > **Generate new token (classic)**.
> 6. **Note:** Give it a name like "MacBook Air Sync."
> 7. **Expiration:** Select "No expiration" (or 90 days if you prefer).
> 8. **Scopes (Permissions):** Check the box for **`repo`** (this is all you need).
> 9. Scroll to the bottom and click **Generate token**.
> 
> ![[../z-Attachments/GitHub Token.png|600]]
> 
>  **TOKEN:** "GIEYTCHPEE"_L33Oe0qAhFgFe78b3U8GfV1eBWk1vV1pWSbT
>  
> ---
> 
> ### **IMPORTANT: Copy the Token Now**
> 
> GitHub will show you a long string of characters starting with `ghp_`. **Copy it immediately** and save it in your Obsidian "References" folder. You will never see it again once you leave the page.
> 
> ---
> 
> ### **Final Terminal Command**
> 
> Go back to your terminal and run the push command again:
> 
> ```bash
> git push -u origin main -f
> 
> ```
> 
> * **Username:** `StyledByShiera`
> * **Password:** **Paste that `ghp_` token you just copied.** (Remember: the cursor won't move while you paste—just hit Enter!)
> 
> ---
> 
> ### **My "Grounded" AI Peer Advice:**
> 
> Once this goes through, you won't have to deal with this "handshake" again for a long time. You've done the heavy lifting of organizing your **Shiera 2.0** vault and linking it to the cloud. You are now officially "Tech-Ready" for your first day of study tomorrow.
> 
> **Did the token work? Once you see those "Writing objects: 100%" messages, go check your GitHub profile—you'll see your first green square!**
> 
> Would you like me to show you how to set up the **Obsidian Git** plugin so you never have to type your username/token again?

###### Git PUSH - Obsidian Notes to GitHub
> [!tip]- Terminal Commands - Git Push every changes made
> ![[../z-Attachments/Git Push every changes made.png]]
> 
> ![[../z-Attachments/Git Push command in Terminal.png]]

###### Terminal Command - Goes back to a folder
> [!tip]- Terminal Command - Goes back to a previous folder
> To go back to the previous folder in your terminal, use this command:
> 
> `cd ..`
> 
> ### **How it works:**
> 
> * **`cd`**: Stands for "change directory."
> * **`..`**: Represents the "parent" folder (the one level above where you are now).
> * **Space**: Make sure there is a **space** between `cd` and the dots.
> 
> ---
> 
> ### **Quick Shortcuts for your Roadmap:**
> 
> As you start building **IRAH**, these three will be your most used commands:
> 
> | Command | What it does |
> | --- | --- |
> | `cd ..` | Goes back **one** level. |
> | `cd ../..` | Goes back **two** levels. |
> | `cd -` | Goes back to the **exact last folder** you were in (like a "back" button). |
> 
> **Would you like me to create a "Terminal Cheat Sheet" for the basic commands you'll need when setting up your Bolt.new or Supabase environment?**

###### Terminal won't allow you to push if you save the GHP code in your Obsidian Notes
> [!tip]- Re-push a commit in Terminal
> I mean inside the **Obsidian app** itself!
> 
> Think of **Obsidian** as your "Design Studio" and the **folder on your laptop** as the "Construction Site." They are the same thing, but Obsidian gives you the nice tools to edit the files easily.
> 
> ### **The "Safety Inspector" Fix**
> 
> 1. **In the Obsidian App:** * Look at your file list on the left.
> * Click on the file named **`IRAH - GitHub.md`**.
> * Find the long code that starts with `ghp_` (your token).
> * **Delete that code entirely from the note.** (This is the "prohibited material" the inspector found).
> 
> 
> 2. **Save the note:** (Just clicking away usually saves it in Obsidian).
> 
> ---
> 
> ### **Now, Go back to the Terminal**
> 
> Once the "secret" is deleted from the note, run these 3 commands to tell GitHub the site is now "Clean":
> 
> ```bash
> git add .
> git commit --amend -m "March 1: Day 1 setup (removed secret token)"
> git push -f
> 
> ```
> 
> ![[../z-Attachments/Re-push and amend a commint in terminal.png|600]]
> 
> ---
> 
> ### **Why we use `--amend` and `-f`:**
> 
> * **`--amend`**: This "edits" your last commit. It’s like rewriting a logbook entry to erase a mistake before anyone officially files it.
> * **`-f` (Force)**: This tells GitHub, "I know what I'm doing, please accept this new, clean version of my history."
> 
> ---
> 
> ### **My "Grounded" AI Peer Advice:**
> 
> As a Director handling BPO fit-outs, you wouldn't leave a master key hanging on the front door for everyone to see. That’s what putting the `ghp_` token in your notes was like! GitHub saw it and protected you.
> 
> Once you delete it from the note and run those commands, your "Site Clearance" will be complete.
> 
> **Did the `git push -f` command give you the "Writing objects: 100%" message this time?**





