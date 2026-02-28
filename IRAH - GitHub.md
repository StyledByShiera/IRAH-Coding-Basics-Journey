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

