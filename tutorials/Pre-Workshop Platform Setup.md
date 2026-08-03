# Pre-Workshop Platform Setup — Do This BEFORE Aug 9th 🛠️

**Workshop:** Platform Setup — August 9th, 2026, 4:00 PM EST
**Bring:** Your laptop, fully charged, with these steps already done 

This guide walks through every click to setting up our trading and charting platforms ahead of our workshop. We're getting the "boring" account-opening and install steps out of the way now (some of it takes a few days to process), so our time together on August 9th goes toward actually learning the platforms and troubleshooting any issues, not waiting on approval emails.

---

## Step 1: Open Your Charles Schwab Account

**Start this one first — options approval can take a few business days to come back.**
You usually get an instant account approval, but full verification takes longer.
For international account, there is currently a long waist list for account verification.
You can still paper trade while waiting for account verification. 

1. Go to **[www.schwab.com](https://www.schwab.com)**
2. Click to open a new account, and choose a **individual brokerage account** (this is the standard, everyday investing account — not a retirement/IRA account). You can choose to open those separately if you wish. 
3. Fill in your personal details as prompted (name, address, Social Security Number, employment info, etc.) — this is standard for any brokerage account and Schwab needs it to verify your identity


📍 **Outside the US?** Visit **[international.schwab.com/open-account-intro](https://international.schwab.com/open-account-intro)** instead, click "Open an account," and use the dropdown to check whether Schwab is available where you live. If it's not, suggested alternatives were Interactive Brokers, Questrade, TastyTrade, or Tradezero. One thing to know: the automated workspace script only works with Schwab/thinkorswim — but that's fine. 

---

### Applying for Options Trading — What to Enter

Partway through opening your account, you'll be asked to fill out a questionnaire about your trading experience. This is what decides which "options approval level" you get — i.e., what kinds of options trades you're allowed to place.

Here's what that section of the form actually looks like:

![Schwab experience level questions](https://raw.githubusercontent.com/tradecblood/5_minute_trader_study_group/main/tutorials/images/charles_swaab_trading_experience_levels_example.png)

That screenshot shows what was entered for this section. Here's it broken out field-by-field:

| Section | Field | Example shown above |
|---|---|---|
| Stocks | Knowledge level | Extensive |
| Stocks | Years of experience | 10 |
| Stocks | Average trades per year | 15 |
| Stocks | Average trade amount (nearest thousand) | $1,000 |
| Options | Knowledge level | Extensive |
| Options | Years of experience | 10 |
| Options | Average trades per year | 15 |
| Options | Average trade amount (nearest thousand) | $1,000 |
| Bonds | Knowledge level | Decline to answer |
| Commodities | Knowledge level | Decline to answer |

**A quick, honest note on this:** those numbers are the experience level that the trader challenge informed us was required for account approval, not necessarily a script for you have to copy word-for-word. Other users have entered their experience level as "Good" and still been accepted. This is *your* answers here. 

- **Bonds & Commodities** — select **"Decline to answer"** for both unless you already trade those separately (most of us will select this)

> ⚠️ **Most important step in this whole section:** When the form asks you to choose an **options trading level / strategy**, select **Level 1 — Long Calls & Puts**.
>
> This is the level that lets you *buy* calls and puts — exactly what the 5-minute strategy does. You do **not** need Level 2 (spreads) or Level 3 (uncovered options). Those unlock more complex, riskier strategies we're not using, so there's no reason to apply for them.

Once submitted, Schwab typically reviews and approves (or asks follow-up questions) within a few business days — this is why we want this done *before* the workshop, not during it.

---

## Step 2: Install ThinkorSwim

**Do this once your Schwab account is active** (you don't need Level 1 options approval to finish this step — you can install and log in while that's still pending).

1. Download **[thinkorswim desktop](https://www.schwab.com/trading/thinkorswim/download?msockid=0bd303fa968f613d0dcd116a976f607b)** from Schwab's website. It will download the thinkorswim desktop application on your laptop. This cannot be done on a cell phone, but you can use the thinkorswim app instead (it will not have the exact same user interface as the desktop version).
   
3. Before logging in, you'll land on a setup screen like the one screenshot below. Select 'paperMoney'. Then, click on the settings icon on the bottom left.
   ![ThinkorSwim setup screen](https://raw.githubusercontent.com/tradecblood/5_minute_trader_study_group/main/tutorials/images/thinkorswim_login_screen.png)

4. After you click on the setting icon, you'll land on a window like the one screenshot below.
   ![ThinkorSwim memory usage](https://raw.githubusercontent.com/tradecblood/5_minute_trader_study_group/main/tutorials/images/thinkorswim_login_screen.png)

Here's what each field means and what to put:

| Field | What it is | What to enter |
|---|---|---|
| **Account** | Which broker this workspace connects to | Schwab |
| **Language** | Display language | English |
| **Color Scheme** | Light or dark theme | Dark (most of us use this — but pick whichever is easier on your eyes) |
| **Proxy** | Network routing setting most people never touch | Leave blank, unless your work/school network specifically requires one |
| **Memory Usage (MB)** | How much of your computer's memory (RAM) thinkorswim is allowed to use. This takes both a minimum and maximum figure. Set them to the same value. | See below 👇 |

**Memory Usage — how to pick a number:**

1. Check how much total RAM your laptop has:
   - **Windows:** right-click the Start button → System → look for "Installed RAM"
   - **Mac:** click the Apple menu (top-left) → About This Mac → look for "Memory"
2. Use this rough guide based on what you find:

| Your laptop's total RAM | Set Memory Usage to |
|---|---|
| 8GB | 2000–3000 MB |
| 16GB | 4000–6000 MB |
| 32GB or more | 6000–8000 MB |

Don't set it to your full RAM amount — leave some room for your browser, Zoom, email, etc. to keep running smoothly at the same time. (The number in the screenshot above is just what worked on one specific laptop — base yours on your own machine, not that exact figure.)

As mentioned above, you can set both values to the same number.


3. Click **Save**.
   💡 If thinkorswim ever runs slow or acts glitchy later on, come back to this same screen and click **"Clear cache and restart"** — that fixes most hiccups.
   
5.  Go back to the thinkorswim login page. Log in using your Charles Schwab account username and password
6. If you bought the Starter Kit (which includes a ready-made script) — or if you built your own custom script — this is where you'll upload it, inside thinkorswim. You can find the custom script built by our group here:  ![ThinkorSwim Workspace Setup](https://raw.githubusercontent.com/tradecblood/5_minute_trader_study_group/main/tutorials/thinkorswim_workspace_setup.md)
   
---

## Step 3: TradingView (quick — just create the account for now)

Go to TradingView and set up a free account so it's ready to go. We'll build out chart layouts, indicators, and drawing tools together, live — no need to configure anything yet, just get the account created.

- Optionally, you can sign up for the TradingView subscription here: [TradingView subscription sign-up](https://www.tradingview.com/pricing/) The cheapest plan is around $12.95.
- You will also need an additional subscription to have live prices on your chart - which is **essential** if you want to use TradingView for  your technical analysis and charting when live or paper trading. But, if your goal is to learn the strategy first, the free version is just fine. The link to subscribe is here, then select "CME Group (E-mini included) CME, CBOT, COMEX, NYMEX"  [subscribe to thinkorswim cme live price data](https://www.tradingview.com/cme/)
- You can **use our admins discount link here for $15 off your subscription**: [Get $15 off TradingView subscription](https://www.tradingview.com/pricing/?share_your_love=teamblood)

---

## Quick Checklist Before Aug 9th

- [ ] Schwab brokerage account opened
- [ ] Options approval application submitted — requested **Level 1 (Long Calls & Puts)**
- [ ] thinkorswim downloaded, installed, and logged in
- [ ] Starter Kit script or your own custom script uploaded in thinkorswim (if applicable)
- [ ] TradingView account created
- [ ] Laptop charged and ready to bring to the call

See you on the 9th! 🚀
