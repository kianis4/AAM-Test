# STUDY GUIDE: GAI — Great American Insurance Program

### *MHCCA Internal Training Guide*

---

## WHAT IS THIS DOCUMENT ABOUT?

The **Great American Insurance (GAI) program** is a game-changer for MHCCA's operations. Launched **December 15th, 2024**, it allows MHCCA to **fund transactions without having to get proof of insurance from the client first.** GAI provides protection from Day 1 of the contract, and then handles the insurance follow-up after funding.

Think of it this way: before GAI, every deal was bottlenecked at funding because you had to chase down the client's Certificate of Insurance (COI) before you could release funds. Now, for qualifying deals, GAI covers you immediately — the client gets funded faster, and the insurance chase happens in the background.

**Why should you care?** Insurance delays are one of the top reasons deals stall at funding. GAI removes that friction for qualifying transactions. But you need to know exactly which deals qualify and which don't — because if a deal DOESN'T qualify for GAI, you still need the traditional insurance process. Getting this wrong means either unnecessarily delaying a GAI-eligible deal or, worse, funding a non-eligible deal without insurance protection.

**Project Owners:** Anne-Sophie Sédillot and Cynthia Gauthier

---

## SECTION 1: HOW GAI WORKS

Here is the timeline for a GAI-covered transaction:

| Timeline | What Happens |
|---|---|
| **Day 1 (Funding)** | MHCCA funds the deal. GAI provides coverage from the start. No COI needed from client. |
| **Days 1-60** | GAI follows up with the client to get their own insurance policy |
| **Day 60 (if no client insurance)** | GAI **automatically bills the client** for insurance coverage (per the Insurance clause in all MHCCA contracts) |
| **After Day 60** | Only a valid proof of insurance meeting MHCCA requirements triggers a **reimbursement process** (date of coverage is considered for calculating reimbursement) |
| **During contract term** | GAI handles insurance **renewal process** |
| **If a claim occurs** | GAI handles **Claims** |

> **Why This Matters:** The 60-day window is critical. The client has 60 days to provide their own insurance. After that, GAI force-places coverage and bills the client. If the client later provides valid insurance, GAI will reimburse them — but only from the date their coverage started, not retroactively to Day 1.

---

## SECTION 2: THE 4 REQUIREMENTS — ALL MUST BE MET

A transaction must meet **ALL 4 requirements** simultaneously to qualify for GAI. Fail any one, and traditional insurance (client COI) is mandatory.

| # | Requirement | Threshold |
|---|---|---|
| 1 | **Not an assignment** | Contract must be a new/original contract |
| 2 | **Contract value < $1MM** | Under one million dollars |
| 3 | **Term between 12 and 84 months** | Minimum 12, maximum 84 months |
| 4 | **100% covered assets** | ALL assets on the contract must be covered (see below) |

### What "100% Covered Assets" Means

Both conditions must be true:
- **100% of assets are non-plated** (no licensed road vehicles)
- **0% of assets generate a Vision automated warning** based on the asset category

Some equipment categories are **excluded** from GAI coverage entirely. Examples include:
- Aircraft
- Drones
- Other specific categories

If even ONE asset on the contract falls into an excluded category, the **entire contract** does not qualify for GAI.

The Vision system warns you: when you flip a deal from "Doc Review" to "Validation" and to "Funding," a warning will appear if any asset category is excluded from GAI.

> **Why This Matters:** The test will likely present a scenario and ask if GAI applies. Check ALL 4 requirements:
> - Is it an assignment? → If yes, no GAI.
> - Over $1MM? → If yes, no GAI.
> - Term outside 12-84 months? → If yes, no GAI.
> - Any excluded or plated assets? → If yes, no GAI.

---

## SECTION 3: VISION SYSTEM INTEGRATION

| Feature | Details |
|---|---|
| **Warning** | Vision generates a warning when a contract **isn't** covered by GAI (meaning you need client COI) |
| **Insurance Tab checkbox** | New checkbox automatically ticked if file is covered by GAI |
| **Purpose** | Identifies contracts that need to be sent to GAI |
| **Override** | You can always **untick** the checkbox to override if needed |

---

## SECTION 4: THE EXCAVATOR EXCEPTION

This is the trickiest part of the GAI program and a very likely test question.

**The situation:** Excavators under categories "heavy" and "small machinery" **ARE covered by GAI.** However, Vision will show a **false warning** saying the contract isn't covered. Why? Because excavators are **plated in Quebec** (they need license plates to operate on roads in Quebec), and the system can't differentiate between provinces for this rule. The system rule can't be modified for **VIN match tracking purposes.**

### What to Do When You See the Excavator Warning

| Province | Action |
|---|---|
| **Quebec** | In the **Insurance tab**, check the **automated insurance program box** |
| **All other provinces** | In the **Equipment tab**, uncheck the **plated box** |

> **Why This Matters:** This is a classic "exception to the exception" that's highly testable. Excavators ARE covered by GAI, but the system says they're not. You need to manually override — and the override method is DIFFERENT depending on whether the deal is in Quebec or another province. Quebec = Insurance tab. Other provinces = Equipment tab.

---

## SECTION 5: HANDLING COIs ON GAI-COVERED CONTRACTS

Even when GAI covers a contract, clients may still send you their Certificate of Insurance. Here's what to do:

### Scenario A: COI Received BEFORE Funding

| Step | Action |
|---|---|
| 1 | Sales Support or Sales Operation sends the COI directly to **GAI** |
| 2 | Email to: **5860.VerifyInsurance@gaig.com** |
| 3 | Include the **contract number** in the email |
| 4 | Sales Support adds a **note in the Audit request template** to let V2 know this step was completed |
| 5 | Do **NOT** validate the content of the COI — GAI handles this |
| 6 | Do **NOT** integrate insurance data in Vision |

### Scenario B: COI Received AFTER Funding

| Step | Action |
|---|---|
| 1 | Sales Support or Sales Operation sends the COI directly to **GAI** |
| 2 | Email to: **5860.VerifyInsurance@gaig.com** |
| 3 | **CC:** **insuranceca@mhccna.com** |
| 4 | Include the **contract number** in the email |

### Key Differences Between Pre-Funding and Post-Funding

| Detail | Pre-Funding | Post-Funding |
|---|---|---|
| Email to GAI | Yes | Yes |
| CC to MHCCA insurance | No | **Yes** (insuranceca@mhccna.com) |
| Add note in Audit request | Yes | Not specified |
| Validate COI content | No — GAI does it | No — GAI does it |
| Integrate in Vision | No | No |

> **Why This Matters:** The big rule for both scenarios: **you do NOT validate the COI yourself and you do NOT enter it in Vision.** GAI handles all insurance validation. The only difference between pre- and post-funding is that post-funding, you CC the MHCCA insurance team (insuranceca@mhccna.com).

---

## SECTION 6: KEY CONTACT INFORMATION

| Contact | Email | Purpose |
|---|---|---|
| **GAI Insurance** | 5860.VerifyInsurance@gaig.com | Send COIs, insurance queries |
| **MHCCA Insurance Team** | insuranceca@mhccna.com | CC on post-funding COIs |
| **MHCCA Insurance (Transfers)** | assurance@mhccna.com | Looped in on transfers (NOT for GAI-covered) |

---

## SECTION 7: QUICK DECISION GUIDE

```
New contract arrives → Check all 4 requirements:

1. Is it an assignment?           → YES = No GAI (need client COI)
2. Is contract ≥ $1MM?           → YES = No GAI
3. Is term outside 12-84 months? → YES = No GAI
4. Any excluded/plated assets?   → YES = No GAI (but check excavator exception!)

ALL 4 requirements met → GAI APPLIES
├─ No need for client COI before funding
├─ GAI checkbox should be ticked in Vision Insurance tab
├─ If client sends COI anyway → forward to GAI, don't validate it yourself
└─ Fund the deal!
```

---

## SECTION 8: WHAT GAI DOES NOT COVER

To be clear, GAI does NOT apply in these situations:

| Situation | Why |
|---|---|
| **Assignment contracts** | Not original contracts |
| **Contracts ≥ $1,000,000** | Above the dollar threshold |
| **Terms < 12 months or > 84 months** | Outside the term window |
| **Plated equipment** | Licensed road vehicles (except excavators — see exception) |
| **Excluded equipment categories** | Aircraft, drones, and other specific exclusions |
| **Mixed contracts with excluded assets** | If even ONE asset is excluded, the whole contract fails |

In all these cases, the **traditional insurance process applies** — you need the client's COI before funding.

**Note:** The full equipment exclusion list is maintained in Vision by equipment category. When a deal is flipped from "Doc Review" to "Validation" to "Funding," Vision will auto-warn you if any category is excluded. You do NOT need to memorize the full exclusion list — the system catches it. But you DO need to know that aircraft and drones are excluded, and that excavators trigger a false warning (see Section 4).

---

## PRACTICE QUESTIONS & ANSWERS

Test yourself. Cover the answers and try to answer from memory.

---

### Question 1
**What is the GAI program, and when was it launched?**

**Answer:** The Great American Insurance program allows MHCCA to fund transactions without requiring proof of insurance from the client first. GAI provides coverage from Day 1. It was launched **December 15th, 2024.**

---

### Question 2
**List all 4 requirements for a transaction to qualify for GAI coverage.**

**Answer:**
1. Contract is **not an assignment**
2. Contract value is **under $1MM**
3. Contract term is between **12 and 84 months**
4. Contract has **100% covered assets** (all non-plated, no excluded categories)

---

### Question 3
**A new contract is for $800,000 of construction equipment (non-plated) on a 60-month term. Does GAI apply?**

**Answer:** **Yes**, assuming it's not an assignment. All 4 requirements are met: not an assignment (assumed), under $1MM ($800K), within 12-84 months (60), and 100% non-plated covered assets.

---

### Question 4
**A contract includes a $500,000 excavator and a $100,000 drone. Does GAI apply?**

**Answer:** **No.** Even though the excavator would normally be covered, the drone is an **excluded equipment category**. Since 100% of assets must be covered and the drone is excluded, the entire contract fails the GAI eligibility check. Traditional insurance (client COI) is required.

---

### Question 5
**What happens after 60 days if the client has not provided their own insurance on a GAI-covered contract?**

**Answer:** GAI **automatically bills and collects from the client** for insurance coverage, as provided by the Insurance clause in all MHCCA contracts. The coverage is force-placed.

---

### Question 6
**A client on a GAI-covered contract provides their own insurance on Day 75. Will they receive a full reimbursement from Day 1?**

**Answer:** **No.** GAI will process a reimbursement, but they take the **date of coverage** into consideration. The client would be reimbursed from the start date of their own policy, not retroactively from Day 1.

---

### Question 7
**An excavator contract in Quebec shows a Vision warning that it's not covered by GAI. What should you do?**

**Answer:** This is a **false warning** — excavators ARE covered by GAI. In **Quebec**, go to the **Insurance tab** and check the **automated insurance program box** to override the warning. (For other provinces, you would uncheck the plated box in the Equipment tab instead.)

---

### Question 8
**An excavator contract in Ontario shows the same false warning. What's different about the fix?**

**Answer:** For **Ontario** (and all other provinces outside Quebec), go to the **Equipment tab** and **uncheck the plated box**. Quebec uses the Insurance tab; all other provinces use the Equipment tab.

---

### Question 9
**A client sends you their COI before funding on a GAI-covered contract. What do you do?**

**Answer:**
1. Send the COI to GAI at **5860.VerifyInsurance@gaig.com** with the contract number
2. Add a note in the **Audit request template** to let V2 know
3. Do **NOT** validate the COI content (GAI does this)
4. Do **NOT** integrate insurance data in Vision

---

### Question 10
**Same scenario, but the COI arrives after funding. What's different?**

**Answer:** Same process, except you also **CC insuranceca@mhccna.com** (the MHCCA insurance team). Pre-funding, you only email GAI. Post-funding, you email GAI AND CC the internal insurance team.

---

### Question 11
**A new (non-assignment) contract is for $1,200,000 of non-plated equipment on a 48-month term. Does GAI apply? Why or why not?**

**Answer:** **No.** While 3 of the 4 requirements are met (not assignment, within 12-84 months, 100% covered assets), the contract value of $1,200,000 **exceeds the $1MM threshold**. ALL 4 requirements must be met simultaneously.

---

### Question 12
**True or False: When you receive a COI on a GAI-covered contract, you should validate the coverage details and enter them into Vision.**

**Answer:** **False.** You do NOT validate the COI content and you do NOT integrate insurance data in Vision. You simply forward the COI to GAI at 5860.VerifyInsurance@gaig.com. GAI handles all validation.

---

### Question 13
**Why does the excavator warning appear in Vision even though excavators are covered by GAI?**

**Answer:** Because excavators are **plated in Quebec** (they need license plates for road operation), and the system can't differentiate between provinces for this rule. The rule can't be modified for **VIN match tracking purposes**, so the warning appears for all excavator deals regardless of province.

---

### Question 14
**What 3 things does GAI handle during the life of a contract?**

**Answer:**
1. **Insurance follow-up** with clients after funding (including force-placement after 60 days)
2. **Renewal process** during the contract term
3. **Claims** management

---

*Source: MHCCA GAI - Validation Guidelines, December 2024. Project Owners: Anne-Sophie Sédillot and Cynthia Gauthier.*
