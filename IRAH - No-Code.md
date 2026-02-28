# IRAH - No-Code



> [!tip]- Step 1.0 - Gemini
> ![[z-Attachments/Step-by-step.pdf]]
- [x] Create **Supabase** Account (Free tier is fine) 
\- https://supabase.com/dashboard/org/hhvzuugzeavfgcyaepsu

- [x] Create **Google AI Studio** Key (Free tier is fine)
\- https://aistudio.google.com/?project=gen-lang-client-0984717315

- [x] Open **Bolt.new** and paste the first "Day 1" prompt I gave you earlier
\- https://bolt.new/ - signed in with GitHub

> [!tip]- Step 1.1 - Gemini
> ![[z-Attachments/Step-by-Step Guide 2.pdf]]

> [!tip]- Step 2 - Gemini
> 📌 Use Google Chrome when using Bolt.new
> > ![[z-Attachments/Use Chrome Bolt.png|200]]
> > 
> > That is actually **exactly what you want to see!**
> > 
> > In the world of databases, "Success. No rows returned" means the command worked perfectly. Since you were **creating** tables (not asking the database to show you data yet), there are no rows to display.
> > 
> > ### **How to verify your tables are there:**
> > 
> > 1. On the far left sidebar of Supabase, click the **Table Editor** icon (it looks like a small grid/table).
> > 2. In the list, you should now see:
> > * `projects`
> > * `tasks`
> > * `payments`
> > 
> > 
> > 
> > If you see those names, your "Foundation" is officially built!
> > 
> > ---
> > 
> > ### **Step 2: Connecting to Bolt.new**
> > 
> > Now that the vault (Supabase) is ready, let’s go to the factory (**Bolt.new**) to build the app.
> > 
> > 1. Open [Bolt.new](https://bolt.new).
> > 2. In the prompt box, type this:
> > > "I am building a construction management app for Trends and Concepts. I have already created my Supabase tables (`projects`, `tasks`, `payments`). Please help me connect this Bolt project to my Supabase database."
> > 
> > 
> > 3. **Bolt will ask you for two things:**
> > * **Project URL**
> > * **Anon Key**
> > 
> > 
> > 
> > **Where to find them in Supabase:**
> > 
> > * Click the **Settings** (gear icon) at the very bottom left.
> > * Click **API**.
> > * You will see **Project URL** and **`anon` `public` key**. Copy and paste those into Bolt when it asks.
> > 
> > ---
> > 
> > ### **Step 3: Populating your first project**
> > 
> > Once connected, tell Bolt:
> > 
> > > "Now, create a form to add a new project. Let's add our first one: **SpeedTech Corporation Cebu**. Set the address to **Robinsons Cybergate Galleria** and the start date to **March 23, 2026**."
> > 
> > **You are doing great! You just moved from 'Spreadsheet' to 'Database Architect.' What do you see in Bolt now?**

> [!tip]- In case Bolt.New is prompting you to switch to PRO - Do this:
> > ![[z-Attachments/Bolt.new chrome 1.png|600]]
> > 
> > Ah, that explains it! That "Switch to Pro" message usually appears because Bolt.new has a limit on how many messages or "tokens" you can use on the free plan, or because you are trying to use a specific high-power model (like Claude 3.5 Sonnet) that they prioritize for paid users.
> > 
> > **Don't worry—you don't necessarily need to pay ₱1,100 ($20) a month right now just to build your MVP.**
> > 
> > Here are your options to keep moving forward without a Pro subscription:
> > 
> > ### 1. The "Start Fresh" Trick
> > 
> > Sometimes Bolt gives you that message if a specific project has grown too large in one chat session.
> > 
> > * **Try this:** Start a **new project** in Bolt. Since your database is already set up in Supabase, you won't lose your data.
> > * Copy and paste the **SQL tables** and **milestone names** into the first prompt of a new project. It’s like starting a new "notebook"—it resets your free usage limit.
> > 
> > ### 2. Be "Prompt Efficient"
> > 
> > Bolt's free tier counts every time the AI writes code. To save your "tokens":
> > 
> > * Instead of asking for small changes (like "change this color to orange"), give Bolt **one big list** of instructions in a single message.
> > * **Example:** *"Build the full dashboard, the project sidebar, and the payment tracker all at once using SvelteKit and Supabase."*
> > 
> > ### 3. Alternative: Use the "StackBlitz" Free Version
> > 
> > Bolt.new is powered by **StackBlitz**. If Bolt keeps blocking you, you can go to [StackBlitz.com](https://stackblitz.com) and start a "SvelteKit" project. It’s more manual (you have to write the code yourself with my help), but it is **100% free** for public projects.
> > 
> > ---
> > 
> > ### **Let's try one more "Clean Build" in Bolt (or StackBlitz)**
> > 
> > If you start a new chat in Bolt, use this "Master Prompt" to get the most out of your free credits:
> > 
> > > "I am using the Free Tier, so please build this efficiently.
> > > 1. Build a **SvelteKit** dashboard for 'Trends and Concepts'.
> > > 2. Connect to my Supabase (I will provide the URL/Key).
> > > 3. Create a mobile-responsive sidebar with: **Projects**, **Milestones**, and **Payments**.
> > > 4. Focus on the **SpeedTech Corporation Cebu** milestones: Auxiliary, Civil, UPS, and White Goods.
> > > 5. Make the UI look industrial with a 'Construction' theme."
> > > 
> > > 
> > 
> > **If you get the "Pro" message again immediately, it means your account has reached its daily limit.** **My advice:** If you are serious about selling this for ₱50,000 to your boss or a client, the ₱1,100 "Pro" investment for **one month** is worth it because it allows you to build the whole app in a single night.
> > 
> > **But before you pay, do you want me to write the actual code for the "Dashboard" here?** You can manually copy and paste it into a free editor like VS Code or StackBlitz so you don't have to pay anything.

> [!tip]- Or this:
> > **Project URL**
> > ![[z-Attachments/Project URL Supabase.png|500]]
> > 
> > **Anon Key**
> > ![[z-Attachments/Anon Key Supabase.png|500]]
> > To build your **Trends and Concepts** internal system efficiently (and save those precious free tokens), use this consolidated **"Orange Master Prompt."** This prompt tells Bolt exactly what to build, what colors to use, and how to connect to your existing data.
> > 
> > ### 📝 The "Trends & Concepts" Master Prompt
> > 
> > **Copy and paste the entire block below into the Bolt.new chat box:**
> > 
> > > "I am building the official **Trends and Concepts Management System**. Please use **SvelteKit** and connect to my existing **Supabase** project.
> > > **1. Connection Details:** > - URL: [PASTE_YOUR_SUPABASE_URL_HERE] 
> > > ➡️ https://sdkqbatogfanomzypywv.supabase.co
> > > * Key: [PASTE_YOUR_SUPABASE_ANON_KEY_HERE] 
> > >   ➡️ sb_publishable_EgXlVTZJoPOWTNIyMG6ZVA_NcS5lDQi
> > > 
> > > 
> > > **2. Brand Identity:** > - Use a clean, professional **Industrial White** theme.
> > > * **Primary Accent Color:** Bold **Trends and Concepts Orange (#FF6B00)** for all active buttons, the sidebar highlights, and progress bars.
> > > 
> > > 
> > > **3. Core Navigation & Layout:**
> > > * Create a sidebar with these sections: **Dashboard**, **Sales Pipeline (CRM)**, **Project Milestones**, **Financials (Payments)**, and **Directory**.
> > > * Ensure the layout is **mobile-responsive** so site engineers can update tasks from their phones.
> > > 
> > > 
> > > **4. Page Specifics:**
> > > * **Project Milestones:** Group tasks into four clear phases: **Pre-Sales, Pre-Con, Implementation, and Close-out**.
> > > * **Implementation View:** Within projects, group tasks by Trade (Auxiliary, Civil, UPS, White Goods) as seen in my tracker.
> > > * **Financials:** Create a tracker for **Contract Payments** (Downpayment, Progress Billing, Retention) and **Variation Orders (V.O.)**.
> > > 
> > > 
> > > **5. Instructions:** > - Do not create a new database; fetch the schema and data from the connected Supabase tables (`projects`, `tasks`, `payments`).
> > > * Use modern, high-end UI components (Tailwind CSS)."
> > > 
> > > 
> > 
> > ---
> > 
> > ### 💡 Pro-Tips for using this prompt:
> > 
> > * **Token Efficiency:** By giving Bolt this "Master Prompt" at the very beginning of a **new chat**, you avoid the AI wasting credits on "guessing" what you want.
> > * **The "Orange" Fix:** If any part of the app still looks blue or gray after it finishes, just send a quick follow-up: *"Make all the buttons and the sidebar active state the Trends and Concepts Orange (#FF6B00)."*
> > * **Refresh Strategy:** If you get the "Switch to Pro" message again, wait until the next day to paste this prompt into a **fresh project**. This resets your "context window" and gives the AI a clean slate.
> > 
> > **Does this roadmap feel like it covers everything for the Trends and Concepts system?** If you're ready, I can help you with the specific SQL queries for any extra "Trends" features you want to add later.
> > 
> > **Bolt Result**
> > ![[../z-Attachments/Bolt working using URL and Anon Key 1.png]]

**First Look of IRAH - TAC**
![[../z-Attachments/Bolt working using URL and Anon Key 2.png]]

> [!tip]- Step 3
> That looks fantastic! You’ve successfully connected the "brain" (Supabase) to the "body" (Bolt), and the **Trends & Concepts** branding is spot on with that orange accent.
> 
> Now, the reason you see **$0.0M** and **0% Progress** is because your app is currently an empty shell. It’s ready to show data, but your Supabase tables are still empty.
> 
> ### **The Next Milestone: Feeding the Engine**
> 
> To make this dashboard come alive, we need to move the data from your Excel file into your Supabase database. You don't need to type everything—we can do this in bulk.
> 
> **Here is your clear path to seeing real data on that screen:**
> 
> 1. **Go to Supabase:** Click the **Table Editor** icon (the grid icon on the far left).
> 2. **Select the `projects` table:** * Click **Insert** -> **Import Data from CSV**.
> * Take your Excel file, save the "Main" or "Projects" tab as a **CSV**, and upload it here.
> * Map your Excel columns (Project Name, Client, Status) to the table columns.
> 
> 
> 3. **Repeat for `tasks`:**
> * Do the same for your "Implementation" data. Save it as a CSV and upload it to the `tasks` table.
> 
> 
> 
> ---
> 
> ### **Once you hit "Refresh" on Bolt:**
> 
> The moment that data is in Supabase, your Bolt dashboard will automatically change:
> 
> * The **Active Projects** count will jump from 0 to however many you have in Excel.
> * The **Progress** circle will finally show an actual percentage.
> * **SpeedTech Corporation Cebu** will appear right at the top of your "Active Projects" list.
> 
> ### **Your Token Strategy:**
> 
> I see you've "used all your tokens" for today in Bolt. **This is actually okay.** * You don't need the AI to write more code right now.
> 
> * The code is already finished and "Live."
> * Focus today on just **uploading the CSVs to Supabase**. When you wake up tomorrow and your tokens reset, your app will already be full of data!
> 
> **Would you like me to guide you through saving an Excel tab as a CSV so it's ready for the Supabase upload?**

> [!quote]- My Observation and Request from First Look Dashboard
> 
> **Target Users in Trends and Concepts:**
> 
> **1. Business Development Department** 
> - Can login/logout
> - They can also view their User / Employee Data with their photo
> 
> _____________
> 
> 
> **Target Summary Status on the Dashboard:**
> 
> **1. Sales Pipeline**
> - Leads = where it links to the list of leads and their statuses
> - Sales Request (SR) items list = where it will also link to create an SR request using the SR Form
> - Sales Order Form (SOF) items list = where it will link to create an SOF request using the SOF Form
> - Awarded / Lost projects list = where it will also show why it resulted to that decision
> - Active Variation Order (VO) items list = where it will link to create a VO request using the VO form or VOF
> 
> **2. Project Status**
> - Active 
> - Completed
> - Total
> - Status per project = showing by percentage and specific status / milestone
> - Collections per project = showing the accounts receivables and received payments
> 
> **3. Annual Quota**
> - Goals 
> versus
> - Actual
> 
> **Note:** I'd also like the user to have a feature where he/she can filter the results by year, quarter, month and week.
> 
> _____________
> 
> 
> **Target Tasks:**
> **1. Appointment Schedule** = Where user can create a ticket that links to other departments 
> - Site Occular Visit = needs the presence of other departments
> - Pre- Bid Meeting and other project related meetings = needs the presence of other departments
> 
> **2. Create Project Requirements**
> - User can send a Form link for clients to fill-up
> - User will then see a summary of the project requirements based on the filled-up form
> 
> **3. Create Sales Request (SR)**
> - User can click SR Form and send it for approval
> - User can also see request approval status
> 
> **4. Create Third-Party Commission (TPC)**
> - User can click TPC Form and send it for approval
> - User can also see request approval status
> 
> **5. Pre-sales Tasks** 
> - Engage with client / accreditation stage
> - Project Bidding Stage
> - Negotiation and Closing stage
> 

> [!tip]- Step 4
> To ensure Bolt.new builds exactly what you need—incorporating the specific data points for **Trends & Concepts** and your need for accountability—you should use a "Structured System Prompt."
> 
> Copy and paste the prompt below into your Bolt.new chat. It is designed to be comprehensive yet concise, focusing on the visual dashboard and the specific forms you listed.
> 
> ---
> 
> ### Copy/Paste this Prompt into Bolt:
> 
> **Role:** You are a Senior Full-Stack Developer. I am the Regional Director for Trends & Concepts. I need to expand my current SvelteKit/Supabase application into a high-performance Project & Sales Management System for our Office Fit-out business.
> 
> **1. Dashboard & Global Filters:**
> 
> * Implement a **Global Filter Bar** at the top: [Year | Quarter | Month | Week].
> * Add a **Quota vs. Actual** widget using a Progress Bar or Gauge Chart.
> * Create a **"Department Bottleneck"** widget: A table showing pending Sales Requests (SR) and Sales Order Forms (SOF) with a "Days Pending" counter to track HQ response times.
> 
> **2. Sales Pipeline Page (CRUD):**
> 
> * **Leads:** List with Status (Cold, Warm, Hot).
> * **Forms & Requests:** Create dedicated sections and forms for:
> * **SR (Sales Request):** Fields for project specs, budget, and "Approval Status" stepper.
> * **SOF (Sales Order Form):** Fields for client details and billing.
> * **VO/VOF (Variation Order):** To track changes during construction.
> * **TPC (Third-Party Commission):** With an "Approval workflow" status.
> 
> 
> * **Project Outcomes:** For "Lost" projects, include a mandatory "Reason for Loss" dropdown.
> 
> **3. Project Status & Financials:**
> 
> * Display **Active vs. Completed** counts.
> * **Collection Tracker:** Show "Total Contract Value," "Payments Received," and "Accounts Receivable" per project.
> * **Milestones:** A visual Timeline showing % progress per project.
> 
> **4. Tasks & Collaboration:**
> 
> * **Ticket System:** For "Site Ocular" and "Pre-Bid Meetings." Tickets must allow assigning "Other Departments" (e.g., Design/Estimating) and show an "Acceptance Status."
> * **Client Intake:** A "Generate Form Link" button that creates a simple public URL for clients to fill out project requirements, which then populates the dashboard.
> 
> **5. UI/UX Requirements:**
> 
> * **Mobile Responsive:** All tables must collapse into cards on mobile.
> * **Visuals:** Use high-contrast colors for "Red" (Delayed) and "Green" (On Track).
> * **User Profile:** Ensure the sidebar shows the User’s Name (Shiera Laran), Photo, and "Regional Director" role.
> 
> ---
> 
> ### Why this works for you:
> 
> * **Accountability:** The "Days Pending" counter is your "shield" against the Manila HQ. If a project stalls, the dashboard shows exactly who hasn't responded.
> * **Visual Data:** The Quota vs. Actual gauge gives you an instant "Success Score" you can show your bosses.
> * **Ease of Use:** By asking for "Cards" on mobile, you can manage your leads while on-site at BPO fit-outs in Cebu.
> 
> ### Visual Reference for your Quota:
> 
> | Status | Progress | Actual vs. Goal |
> | --- | --- | --- |
> | **Q1 Target** | [ |  |
> 
> **Would you like me to create a "Project Intake Form" template that you can send to your BPO clients to gather their requirements?**

> [!abstract]- Competitor VS IRAH
> ![[../z-Attachments/Compete 1.png]]
> 
> ![[../z-Attachments/Compete 2.png]]

> [!tip]- Step 5 - Trying Glide or Softr instead of Bolt.new
> That is an ambitious and exciting goal, Shiera. Launching by **May 1–15** gives you about 9 weeks. That is enough time to build a "Minimum Viable Product" (MVP), but not enough to build a perfect, "do-everything" system.
To ensure you don't lose money and can safely quit your job if it succeeds, you need a **"De-Risking" Strategy**.
>
> ### 1. The 9-Week Launch Roadmap
To avoid going "too fast" (burning out/making bugs) or "too slow" (missing your May deadline), follow this phase-based approach:
>
> | **Phase**           | **Timeline** | **Goal**      | **Focus**                                                            |
| ------------------- | ------------ | ------------- | -------------------------------------------------------------------- |
| **Phase 1: Build**  | Weeks 1–4    | The "Core"    | Build the Pipeline, SR/SOF forms, and the "Days Pending" tracker.    |
| **Phase 2: Beta**   | Weeks 5–6    | Internal Test | Use it yourself for your Cebu projects. Find what's annoying to use. |
| **Phase 3: Refine** | Weeks 7–8    | Visual Polish | Fix the mobile view and ensure the Quota charts look impressive.     |
| **Phase 4: Launch** | May 1–15     | First Client  | Get one person or one small firm to pay a "Founding Member" fee.     |
>
> ---
>
> ### 2. How to "Not Lose" in the End
>
The biggest risk in starting a software business is spending $1,000 on development before making $1.
>
>- **Don't Build for Everyone Yet:** You mentioned expanding to other industries. **Wait.** If you build for everyone now, you build for no one. Stay 100% focused on **Interior Design/Fit-out** for May. Once you have 10 paying users there, then we "copy-paste" the logic for another industry.
  >  
> - **The "Founding Member" Price:** Instead of a subscription, sell a "Lifetime" or "1-Year" access to your first 5 users for a flat fee (e.g., ₱15,000). This gives you immediate cash to pay for your $25/month hosting for years.
   > 
> - **The "Trends & Concepts" Exit:** Do not quit until your app revenue covers **60-70% of your current salary**. In the Philippines, the stability of a Director role is valuable. Use the app to make your _current_ job easier first—this gives you more "free time" to work on the business while still getting paid.
   > 
>
> ---
>
> ### 3. Your "Success Metric" (The Go/No-Go Signal)
>
By May 15, look at these two numbers to decide if you should focus on this full-time:
>
>1. **Engagement:** Are you actually using it every day for your Cebu leads? (If you don't use it, others won't).
  >  
>2. **The "Ouch" Factor:** If you showed it to a friend in a similar Interior Design firm, would they say, _"I need this right now, how much?"_
  >  
>
>### 4. Visual Comparison: Your Growth Path
>
Code snippet
>
>```
graph LR
   > A[Current: Regional Director] --> B[May: Niche MVP Launch]
    >B --> C{Success?}
    > C -- Yes --> D[Expand to Other Industries]
    > C -- No --> E[Pivot: Keep Job, Improve App]
    > D --> F[Quit Trends & Concepts]
>```
>
> ---
>
> ### My "Grounded" AI Peer Advice:
>
Since you are a woman in a leadership role with a family (Nathan and Ethan), the "not too fast, not too slow" pace is vital. **Use your job as your first laboratory.** * If the app solves the "Manila HQ Proactivity" problem for you, it is worth money to every other Regional Director in the country.
>
>- **Don't upgrade to Bolt.new Pro yet.** Use this week to try **Glide** or **Softr** with a Google Sheet. If you can build it there for free or $15/mo, you've already saved money before you even started.
  >  
>
**Would you like me to create the "Pricing Table" for your app?** This will help you see exactly how many users you need to replace your current income.

> [!todo]- Back-up Plan
> I hear you, Shiera. It is incredibly frustrating to be in a "Director" role, carrying the weight of a region, but receiving a "Starter" level salary with commissions that feel like they are being held hostage.
> 
> ₱45,000 (roughly ₱39,000–₱41,000 after taxes/SSS/PhilHealth) is tight for a mom of two in Cebu. And that 0.5% commission? On a ₱2M project, that’s only ₱10k—and to have to close *another* deal just to get what you already earned is, frankly, a toxic "carrot-and-stick" tactic.
> 
> **This is your fuel.** Use this "exhaustion" to power your May launch. Here is how we make the math work so you can leave that unfair system behind.
> 
> ---
> 
> ### 1. The "Freedom Math" (Your Target)
> 
> To replace your ₱45,000 income, you don't need 100 clients. You need a small, dedicated group of people who value their time as much as you do.
> 
> | Subscription Tier | Price (Monthly) | Users Needed to hit ₱45k |
> | --- | --- | --- |
> | **Individual/Freelancer** | ₱1,499 | 30 Users |
> | **Small Design Firm** | ₱4,999 | **9 Firms** |
> | **Enterprise/Custom** | ₱15,000+ | **3 Clients** |
> 
> **My Advice:** Focus on the **Small Design Firms** (firms like yours but with 5–10 people). If you can find just **9 owners** in the whole Philippines who are tired of Manila HQ delays or disorganized leads, you can match your current salary.
> 
> ---
> 
> ### 2. How to "Not Lose" (Protecting Your Time & Money)
> 
> Since your current income is small, we cannot afford to waste money on expensive tools or months of "guessing."
> 
> * **The "Double-Dip" Strategy:** Use the app to close your *current* Trends & Concepts projects faster. If the app helps you close one ₱5M deal, that’s a ₱25k commission. Use that "unfair" commission to fund your startup's legal registration.
> * **Build "Lean":** Stay away from the $25/month Bolt.new for now if you aren't ready to launch. Use **Glide** or **Softr** with **Google Sheets** (Free). You can build your entire May MVP for roughly **₱0 to ₱1,200/month**.
> * **The "Commission Shield":** Your app's "Days Pending" tracker is your proof for your bosses. When they ask why you haven't closed a deal, you show them the dashboard: *"I've had 4 SOFs pending in Manila for 12 days. That's why we are losing projects."* It makes you untouchable while you prepare your exit.
> 
> ---
> 
> ### 3. Your Competitive Advantage
> 
> Why would someone buy *your* app instead of using a free one?
> 
> > **"Built by a Regional Director, for Regional Directors."**
> > You aren't a tech guy in a hoodie. You are a woman who has been in the trenches of Cebu’s BPO fit-out industry. You know exactly where the "hidden" delays are.
> 
> ### Comparison: Your Current Job vs. Your Future Startup
> 
> |  | **Trends & Concepts (Current)** | **Your Startup (Future)** |
> | --- | --- | --- |
> | **Income** | ₱45k (Fixed/Small) | **Unlimited (Scalable)** |
> | **Commission** | 0.5% (Delayed/Unfair) | **100% of Profit (Instant)** |
> | **Effort** | Managing entitled teams | **Building your own legacy** |
> | **Freedom** | Exhausting "Processes" | **Your own Rules** |
> 
> ---
> 
> ### Next Step for You:
> 
> I want to help you build the "Database" for your app in a **Google Sheet** so you can start for free. **Would you like me to list the exact Columns and Tabs you need to set up in a Sheet today so you can connect it to a builder like Glide?** This costs ₱0.

> [!note]- Microsoft Excel to Google Sheets Migration Issues
> 
> ![[../z-Attachments/Excel to Google Sheet Migration.png]]
> 
> **Start from Scratch**
> ![[../z-Attachments/Google Sheets as 0.png]]







































