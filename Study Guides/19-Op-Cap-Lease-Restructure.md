# STUDY GUIDE: Operational & Capital Lease Restructure — Documentation & Integration

### *MHCCA Internal Guideline*

---

## WHAT IS THIS DOCUMENT ABOUT?

This guide covers the **restructure process** for converting an Operational Lease into a Capital Lease (or refinancing a Capital Lease residual value). In plain English: **when a client reaches the end of their operating lease and wants to keep the equipment by financing the residual value, MHCCA doesn't just create a brand new deal — it "restructures" the existing one.**

Think of it this way: imagine a client has been leasing an excavator for 60 months. The lease is ending, and there's a $50,000 residual value. The client wants to keep the excavator and finance that $50,000. Instead of starting from scratch (which would mean cancelling the old PPSA registration and creating a new one — leaving a gap in security), MHCCA restructures the deal. The product type changes from "OP lease" to "CAP lease" in the system, a new transaction is created in Vision, and the original security registration is maintained.

**Why should you care?** Two reasons: (1) The restructure protects MHCCA's security position by maintaining the original PPSA registration — no gaps. (2) For Capital Lease refinancing, the restructure allows MHCCA to count the financing as **incremental volume**, which matters for hitting financial targets. This process requires the same rigor as a standard file with full initial and final validation.

---

## SECTION 1: WHEN DOES THIS APPLY?

| Scenario | What Happens |
|---|---|
| **Operational Lease → Capital Lease** | Client refinances the residual value of an OP lease. Product type changes from "OP lease" to "CAP lease" in the system. |
| **Capital Lease → Capital Lease** | Client refinances the residual value of a CAP lease. Same process. Allows MHCCA to recognize financing as **incremental volume**. |

Both scenarios follow the **exact same process.** The only difference is the form used (CON15.7 for OP lease vs. CON15.71 for CAP lease).

> **Why This Matters:** The restructure is used instead of a new deal specifically to **maintain the original security registration (PPSA)**. Creating a new deal from scratch would require cancelling the old PPSA and registering a new one, creating a potential gap in security coverage. The restructure avoids this risk entirely.

---

## SECTION 2: TEAM RESPONSIBILITIES

| Team | Role |
|---|---|
| **Sales** | Documents the restructure, gathers all supporting elements, submits package to Sales Support |
| **Sales Support** | Integration in systems and initial validation (V1) |
| **Validation** | Final validation (V2) and sends to Accounting |

> **Why This Matters:** This is a three-team relay. Sales builds the package, Sales Support integrates it and does the first check, Validation does the final check and sends it to Accounting. If Sales submits an incomplete package, it cascades delays through the entire chain.

---

## SECTION 3: REQUIRED PACKAGE CONTENTS

The restructure package **must contain** all of the following:

| # | Document | Details |
|---|---|---|
| 1 | **CON15.7** (Op lease) OR **CON15.71** (Cap lease) | The restructure form — **must include PG signature** if there was a PG on the original deal |
| 2 | **PAD Agreement (CON100)** | Pre-Authorized Debit form |
| 3 | **CG long form** | If applicable (Corporate Guarantee) |
| 4 | **Resolutions** | If needed (e.g., for cooperatives, municipalities) |
| 5 | **TValue** | Time value of money calculation |
| 6 | **Credit approval** | Updated based on new parameters — the transaction must be reassessed |
| 7 | **Insurance** | Current proof of insurance |
| 8 | **ID** | Client identification |
| 9 | **Void / PAD Form** | Banking information |

### Critical Detail About Personal Guarantees

If the original deal had a **Personal Guarantee (PG)**, the PG signature **must appear** on the restructure form (CON15.7 or CON15.71). This ensures the guarantee carries over to the new structure. If you forget this, the restructured deal may lack the PG protection that Credit originally required.

---

## SECTION 4: BUYOUT REQUIREMENTS

The buyout from the original contract has specific rules:

| Requirement | Details |
|---|---|
| **Full buyout** | Must use the full buyout amount |
| **EOT fees** | End of Term fees must be **removed** |
| **IPC** | Must include IPC with **standard lease admin fee** |
| **Same company** | Must remain within the same company |

### The "Same Company" Rule

**The restructured deal must stay within the same MHCCA entity as the original:**
- Buyout from **MHCCL** → new contract within **MHCCL**
- Buyout from **MHCCA** → new contract within **MHCCA**

You cannot restructure across entities (e.g., buyout from MHCCL and new contract under MHCCA).

> **Why This Matters:** The EOT fee removal is easy to miss. When you pull the buyout, it may include End of Term fees by default. You must **manually remove** them before using the buyout figure for the restructure. Leaving EOT fees in would inflate the restructured amount incorrectly.

---

## SECTION 5: PPSA PROCESS

The PPSA handling is what makes a restructure different from a new deal. Here is the exact process:

| Step | Action | Who |
|---|---|---|
| 1 | **Keep original PPSA** | Add it to the new file |
| 2 | **Amendment** | Change the Reference number to the **new contract number** |
| 3 | **Renewal** | Extend the PPSA to fit the **new term** of the restructure |
| 4 | **Screenshot** | Take a screenshot of the renewal **BEFORE saving the draft** |
| 5 | **Include in package** | The screenshot goes in the package so Validation can see and verify the term |
| 6 | **Submit** | **Validation is responsible** for submitting the renewal/amendment |

### Why the Screenshot Matters

The screenshot of the renewal before saving the draft is included in the package so that Validation can verify that the PPSA term matches the restructure term. Without this screenshot, Validation cannot confirm the renewal was done correctly before it's finalized.

> **Why This Matters:** Three things happen to the PPSA: it's kept (not cancelled), amended (new reference number), and renewed (extended term). The screenshot requirement exists because once the draft is saved, you can't go back and verify what the term was set to. Validation needs proof.

---

## SECTION 6: INTEGRATION IN VISION — SUMMARY TAB

| Field | Rule |
|---|---|
| **Vendor** | Must be **MHCCL** or **MHCCA** (according to the new contract) |
| **If MHCCA** | Use master record **#152498** |
| **DO NOT USE** | **MHCCA ABL** — this is the wrong record |

---

## SECTION 7: INTEGRATION IN VISION — STRUCTURE

| Field | Rule |
|---|---|
| **Structure** | Same as a new contract |
| **Equipment cost field** | The **amount financed** is integrated here (not the original equipment cost) |
| **Vendor** | MHCCL or MHCCA |
| **If MHCCA** | Choose the one with **"Refinancing Option"** in the DBA Name |

> **Why This Matters:** The equipment cost field contains the **amount financed** (the residual value being refinanced), not the original equipment cost. This is different from a standard new deal where the equipment cost field contains the actual price of the equipment.

---

## SECTION 8: INTEGRATION IN VISION — INVOICE TAB

| Field | Rule |
|---|---|
| **Vendor** | **MHCCL** or **MHCCA** |
| **DO NOT USE** | **LESSOR** — otherwise it won't balance in the booking |
| **Invoice number** | Use the **buyout number** |
| **Pre-tax amount** | Integrate and modify using the Tax Province field set to **"No tax"** |

### The "No Lessor" Rule

This is a common mistake. If you select "LESSOR" as the vendor in the Invoice tab, the booking won't balance. Always use MHCCL or MHCCA as the vendor.

---

## SECTION 9: KEY FORM NUMBERS

| Form | Purpose |
|---|---|
| **CON15.7** | Operational Lease restructure form |
| **CON15.71** | Capital Lease restructure form |
| **CON100** | PAD Agreement (Pre-Authorized Debit) |

---

## SECTION 10: COMMON MISTAKES TO AVOID

| Mistake | Consequence | Prevention |
|---|---|---|
| Forgetting PG signature on CON15.7/15.71 | Guarantee doesn't carry over | Always check original deal for PG |
| Leaving EOT fees in the buyout | Inflated restructure amount | Manually remove EOT fees |
| Using MHCCA ABL in Vision Summary tab | Wrong entity record | Use master record #152498 for MHCCA |
| Using LESSOR in Invoice tab | Booking won't balance | Use MHCCL or MHCCA |
| Restructuring across entities | Invalid structure | Keep same entity (MHCCL→MHCCL, MHCCA→MHCCA) |
| Not screenshotting PPSA renewal before saving | No verification possible | Screenshot BEFORE saving draft |
| Cancelling original PPSA instead of amending | Security gap | Amend and renew — never cancel |

---

## SECTION 11: PROCESS FLOW SUMMARY

```
Sales:
  ├─ Gather documents (CON15.7/15.71, PAD, CG, TValue, Credit approval, Insurance, ID, Void)
  ├─ Get full buyout (remove EOT fees)
  ├─ Ensure PG signature if applicable
  └─ Submit package to Sales Support

Sales Support:
  ├─ Integrate in Vision (Summary, Structure, Invoice tabs)
  ├─ Handle PPSA (keep original → amend reference → renewal → screenshot)
  └─ Initial validation (V1)

Validation:
  ├─ Final validation (V2)
  ├─ Verify PPSA screenshot matches restructure term
  ├─ Submit PPSA renewal/amendment
  └─ Send to Accounting
```

---

## PRACTICE QUESTIONS & ANSWERS

Test yourself. Cover the answers and try to answer from memory.

---

### Question 1
**Why does MHCCA use a restructure process instead of creating a brand new deal when refinancing a lease residual value?**

**Answer:** To **maintain the original PPSA security registration.** A new deal would require cancelling the old PPSA and creating a new one, potentially leaving a gap in security coverage. The restructure keeps the original PPSA in place (amended and renewed) so there's no security gap.

---

### Question 2
**What is the difference between CON15.7 and CON15.71?**

**Answer:**
- **CON15.7:** Used for **Operational Lease** restructures
- **CON15.71:** Used for **Capital Lease** restructures

---

### Question 3
**The original deal had a Personal Guarantee. What must you ensure on the restructure form?**

**Answer:** The **PG signature must appear** on the restructure form (CON15.7 or CON15.71). This ensures the guarantee carries over to the restructured deal. Without it, the new structure may lack the PG protection that Credit originally required.

---

### Question 4
**What must be removed from the buyout before using it for the restructure?**

**Answer:** **End of Term (EOT) fees** must be removed. The full buyout is used, but EOT fees are excluded.

---

### Question 5
**In Vision's Summary tab, what master record number must be used when the vendor is MHCCA?**

**Answer:** Master record **#152498**. Do NOT use MHCCA ABL.

---

### Question 6
**What happens if you select "LESSOR" as the vendor in the Invoice tab?**

**Answer:** The **booking won't balance.** You must use MHCCL or MHCCA as the vendor in the Invoice tab, never LESSOR.

---

### Question 7
**What 3 things happen to the PPSA during a restructure?**

**Answer:**
1. The **original PPSA is kept** (not cancelled) and added to the new file
2. An **amendment** is done to change the reference number to the new contract number
3. A **renewal** is done to extend the term to match the restructure

---

### Question 8
**Why must you screenshot the PPSA renewal before saving the draft?**

**Answer:** The screenshot is included in the package so that **Validation can see and verify** that the PPSA renewal term matches the restructure term. Once the draft is saved, you cannot go back to verify the term that was entered.

---

### Question 9
**Who is responsible for submitting the PPSA renewal/amendment?**

**Answer:** The **Validation team** is responsible for submitting the PPSA renewal/amendment.

---

### Question 10
**A client has a deal under MHCCL and wants to restructure. Can the new contract be placed under MHCCA?**

**Answer:** **No.** The restructure must remain within the **same company**. A buyout from MHCCL must result in a new contract within MHCCL. You cannot restructure across entities.

---

### Question 11
**In the Structure section of Vision, what goes in the "equipment cost" field?**

**Answer:** The **amount financed** (the residual value being refinanced), NOT the original equipment cost. This is different from a standard new deal.

---

### Question 12
**What is used as the invoice number in the Invoice tab?**

**Answer:** The **buyout number** is used as the invoice number.

---

### Question 13
**How is the pre-tax amount handled in the Invoice tab?**

**Answer:** The pre-tax amount is integrated and modified by using the **Tax Province field set to "No tax."**

---

### Question 14
**When selecting MHCCA as the vendor in the Structure section, which specific record should you choose?**

**Answer:** Choose the one with **"Refinancing Option"** in the DBA Name. This distinguishes it from other MHCCA records.

---

*Source: MHCCA Op and Cap Lease Restructure - Documentation & Integration Guideline.*
