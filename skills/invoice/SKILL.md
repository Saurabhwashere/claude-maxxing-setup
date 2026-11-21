---
name: invoice
description: Drafts a client invoice from a few details. Use when I say "invoice", "bill this client", or list work and amounts to charge.
---

# Invoice

## Inputs
- Client name and email.
- What I did (line items) and the price for each.
- Optional: due date (default 14 days), currency (default USD).

## Steps
1. Read `references/my-details.md` for my business name, address and payment info. If it's missing, leave placeholders and tell me.
2. Make the next invoice number: `INV-<YYYY>-<NNN>`. Ask me the last number if you don't know it.
3. Build the invoice as a clean markdown table:

| Item | Qty | Rate | Amount |
|------|-----|------|--------|

4. Add subtotal, tax (only if I give a rate), and total.
5. Add a payment line: due date and how to pay.
6. Write a 2-line email to send with it.

## Rules
- Double-check the maths. Show the total once, bold.
- Never invent prices or line items.
- Never send. Draft only.
